# OBD-II-Eco-driving-assistant

This repository contains codes and datasets in correspondence to my bachelor thesis for computer science at Vrije Universiteit Amsterdam. 

## Datasets
- exp1_14drivers_14cars_dailyRoute.csv -> original data set for the experiment, acquired from the [public dataset](https://github.com/cephasax/OBDdatasets) published by Cephas Barreto. 
- exp2_19drivers_1car_1route.csv -> same as the previous one.

- train_shuffled_16features.csv -> the train set with 16 features after initial data engineering.
- train_shuffled_7features.csv -> the train set with 7 features after selecting important features.
- train_shuffled_43features.csv -> the train set with 43 features after feature crosses.

- test_shuffled_16features.csv -> the test set with 16 features after initial data engineering.
- test_shuffled_7features.csv -> the test set with 7 features after selecting important features.
- test_shuffled_43features.csv -> the test set with 43 features after feature crosses.

- total_16features.csv -> the total set with 16 features before spliting corresponding train and test set.
- total_7features.csv -> the total set with 7 features before spliting corresponding train and test set.
- total_43features.csv -> the total set with 43 features before spliting corresponding train and test set.

- case_study_19drivers.csv -> dataset used for the case study mentioned in Chapter 4 of the thesis.

## Notebooks
- data_preparation_xfeatures.ipynb -> data wrangling and engineering to produce the corresponding dataset.
- data_preparation_case_study.ipynb -> data wrangling and engineering to produce the dataset used in the case study .

- modelling_xfeatures.ipynb -> build regression models according to datasets with different number of features.
- modelling_case_study.ipynb -> case study for 19 drivers as mentioned in Chapter 4 of the thesis.

- automl_1h.ipynb -> 1h training using automl, the dataset and regressor used can be modified accordingly

## Running environment

All codes are written in python and jupyter notebook. Jupyter notebook can be installed following the [official installation guide](https://jupyter.org/install).  

After successfully deployed the jupyter notebook, all notebooks can be compiled directly on python3 for a version higher than 3.9. When compiling, make sure that all documents are in the same directory. There is no requirement for the operating system, with the exception of automl_1h.ipynb.

Automl requires python3 and jupyter notebook to be deployed on a Linux operating system. In order to run automl in other operating systems, possible solutions are WSL for windows, virtual machine, docker image, etc.

