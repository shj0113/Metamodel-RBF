# Metamodel-RBF
Radial Basis Function (RBF)

논문과 관련된 정보 및 githup repository의 목적 포함
Design of Advanced Energy Systems (IDAES)가 scientific community에서 자유롭게 사용 가능한지 명시

## Installation
### Requirements
필요한 패키지 설치(의존성 고려) 

### Virtual environment
We first create a virtual environment to avoid dealing with other packages installed in the system:

Test folder:
$ mkdir Test && cd Test

We create a virtual environment:
$ python -m venv CodeName_venv

And activate it:
$ source ./CodeName_venv/bin/activate

### Dependencies and packages
(CodeName_venv) $ pip install

## Usage
This repository provides two Jupyter Notebooks:
1. **Reproducing the results presented in the paper**
2. **Training and testing the model with new data**

### 1. Reproducing the results from the paper
To reproduce the results presented in the paper, follow these steps:
1. Clone this github repository
2. Run the `RadialBasisFunctions.ipynb`

The required datasets, `curing_time_data.xlsx` and `flexural_strength_data.xlsx`, are located in the `data/` folder. These datasets are from the experimental results in the paper. To fully reproduce Figures 4 and 5 from the paper, simply change the **sheet_name** in the dataset as needed.

### 2. Training and testing with new data
To train and test the model with new data, follow these steps:
1. Clone this github repository
2. Prepare new data
   - The dataset must be structured with the first three columns (x1, x2, x3) representing the input variables, and the last column (y) representing the target variable to be predicted
   - You can refer to the `example_new_data.csv` file located in the `data/` folder.
3. Run the `RadialBasisFunctions_Newdata.ipynb`

## Results


## License
MIT License
