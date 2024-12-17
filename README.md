# Metamodel-RBF
Radial Basis Function (RBF)

논문과 관련된 정보 및 githup repository의 목적 포함
Design of Advanced Energy Systems (IDAES)가 scientific community에서 자유롭게 사용 가능한지 명시

## Contents

## Installation
### Requirements
필요한 패키지 설치(의존성 고려) 

### Virtual Environment
We first create a virtual environment to avoid dealing with other packages installed in the system:

Test folder:
$ mkdir Test && cd Test

We create a virtual environment:
$ python -m venv CodeName_venv

And activate it:
$ source ./CodeName_venv/bin/activate

### Dependencies And Packages
(CodeName_venv) $ pip install

## Usage
This repository provides two Jupyter Notebooks:
1. To reproduce the results from the paper
2. To train and test the model with new data

### 1. Reproducing the Results from the Paper
To reproduce the results presented in the paper, follow these steps:
1. Clone our github repository
2. Run the RadialBasisFunctions.ipynb
The required datasets are located in the data/ folder as CSV files.

### 2. Training and Testing with New Data
To train and test the model with new data, run the following steps:
1. Clone our github repository
2. Prepare new data
   - Format: The new data should be in CSV format
   - Structure: The first three columns represent the input variables. The last column represents the target variable to be predicted.
4. Run the RadialBasisFunctions_Newdata.ipynb

## Results


## License
MIT License
