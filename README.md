# Metamodel-RBF
This repository contains the code for implementing the Radial Basis Function (RBF) model and the dataset used in **"Accentuating the Ambient Curing Behavior of Geopolymers: Metamodel-Guided Optimization for Fast-Curing Geopolymers with High Flexural Strength"** published in [Digital Discovery](https://pubs.rsc.org/en/journals/journalissues/dd#!recentarticles&adv).

This repository serves two main purposes:
1. To reproduce the results presented in the paper by providing the code and dataset
2. To enable the use of the code in optimizing multi-variant problems for targeted properties

This code is implemented based on the IDAES Process Systems Engineering Framework using pyomo, developed by the Institute for the Design of Advanced Energy Systems (IDAES). 

The IDAES libraries used in this work are freely accessible to the scientific community.
- IDAES | [Website](https://idaes-pse.readthedocs.io/en/stable/index.html) | [GitHub](https://github.com/IDAES/idaes-pse)

## Installation
### Requirements
- python = 3.7
- idaes-pse = 1.13.0
  
### Virtual environment
We highly recommend creating a virtual environment using [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) to manage versions and prevent conflicts with other packages.

We create a virtual environment with a name of your choice (in this example, `rbf`):
```
$ conda create -n rbf python=3.7
```
And activate it:
```
$ conda activate rbf
```

### Dependencies and packages
We install the required dependencies and packages using pip:
```
(rbf) $ pip install idaes-pse==1.13.0 
(rbf) $ pip install scipy pandas numpy matplotlib
```


## Usage
This repository provides two Jupyter Notebooks:
1. **Reproducing the results presented in the paper:** `RadialBasisFunctions.ipynb`
2. **Training and testing the model with new data:** `RadialBasisFunctions_Newdata.ipynb`

### 1. Reproducing the results from the paper
To reproduce the results presented in the paper, follow these steps:
1. Clone this github repository
2. Run the `RadialBasisFunctions.ipynb`

The required datasets, `curing_time_data.xlsx` and `flexural_strength_data.xlsx`, are located in the `data/` folder. These datasets are from the experimental results in the paper. To fully reproduce Figures 4 and 5 from the paper, simply change the **sheet_name** in the dataset as needed.

### 2. Training and testing with new data
To train and test the model with new data, follow these steps:
1. Clone this github repository
2. Prepare new dataset
   - The new dataset must be structured with the first three columns **(x1, x2, x3)** representing the input variables and the last column **(y)** representing the target variable to be predicted
   - You can refer to the `example_new_data.csv` file located in the `data/` folder.
3. Run the `RadialBasisFunctions_Newdata.ipynb`

## Results

### RBF models for flexural strength (Figure 4)
![Figure4](https://github.com/user-attachments/assets/4d77b35b-aeab-4df6-b0cf-adbd3308a1de)

### RBF models for curing time (Figure 5)
![Figure5](https://github.com/user-attachments/assets/fd163244-ba2b-45ff-8e24-61cc084338c1)


## License
MIT License
