# Metamodel-RBF
Radial Basis Function (RBF)

논문과 관련된 정보 및 githup repository의 목적 포함
Design of Advanced Energy Systems (IDAES)가 scientific community에서 자유롭게 사용 가능한지 명시

## Installation
### Requirements
- python = 3.7
- idaes-pse = 1.13.0
  
### Virtual environment
We highly recommend creating a virtual environment using [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) to manage versions and prevent conflicts with other packages.

We create a virtual environment with a name of your choice (e.g., `rbf`):
```
$ conda create -n rbf python=3.7
```
And activate it:
```
$ conda activate rbf
```

### Dependencies and packages
Install the required dependencies and packages using pip:
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
   - The new dataset must be structured with the first three columns (x1, x2, x3) representing the input variables and the last column (y) representing the target variable to be predicted
   - You can refer to the `example_new_data.csv` file located in the `data/` folder.
3. Run the `RadialBasisFunctions_Newdata.ipynb`

## Results


## License
MIT License
