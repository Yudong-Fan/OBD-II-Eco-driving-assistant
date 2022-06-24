# OBD-II-Eco-driving-assistant

This repository contains codes in correspondence to my bachelor thesis for computer science at Vrije Universiteit Amsterdam. Specifications for the files are shown below.

## Datasets
- exp1_14drivers_14cars_dailyRoute.csv -> original data set for the experiment, acquired from the [public dataset](https://github.com/cephasax/OBDdatasets) published by Cephas Barreto. 
- exp2_19drivers-1car-1route.csv -> same as the previous one.

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
- data_preparation_case_study -> data wrangling and engineering to produce the dataset used in the case study .

- modelling_xfeatures.ipynb -> building regression models accordingly.
- modelling_case_study -> directly in correspondence to the implementations in Chapter 4 of the thesis.