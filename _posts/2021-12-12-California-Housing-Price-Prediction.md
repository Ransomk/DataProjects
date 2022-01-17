---
title: California Housing Price Prediction
date: 2021-12-12 12:37:00 +0530 
tags: [Machine learning, Python, Exploratory Data Analysis, Linear Regression, numpy, pandas, sklearn, seaborn, matplotlib]
comments: false
img_path: /assets/img/
---

### Summary

The project includes analysis on the California Housing Dataset with some Exploratory data analysis .
There was encoding of categorical data using the one-hot encoding present in pandas.
Also standardization of the data and use of Linear Regression models from sklearn and Seaborn plots

You can view the full project code on this [Github link](https://github.com/Ransomk/California-Housing-Price-Prediction)

Note: _This is an academic project completed by me as part of my Post Graduate program in Data Science from Purdue University through Simplilearn. The project was towards the completion of Data Science with R module._

### Bussiness Scenario
The US Census Bureau has published California Census Data which has 10 types of metrics such as the population, median income, median housing price, and so on for each block group in California. The dataset also serves as an input for project scoping and tries to specify the functional and nonfunctional requirements for it. The project aims at building a model of housing prices to predict median house values in California using the provided dataset. This model should learn from the data and be able to predict the median housing price in any district, given all the other metrics. Districts or block groups are the smallest geographical units for which the US Census Bureau publishes sample data (a block group typically has a population of 600 to 3,000 people). There are 20,640 districts in the project dataset.

### Analysis Steps
1. Load the data :
    - Read the “housing.xlsx” file from the folder into the program.
    - Print first few rows of this data.
    - Extract input (X) and output (Y) data from the dataset.
2. Handle missing values :
    Fill the missing values with the mean of the respective column.
3. Encode categorical data :
    Convert categorical column in the dataset to numerical data.
4. Split the dataset :
    Split the data into 80% training dataset and 20% test dataset.
5. Standardize data :
    Standardize training and test datasets.
6. Perform Linear Regression :
    - Perform Linear Regression on training data.
    - Predict output for test dataset using the fitted model.
    - Print root mean squared error (RMSE) from Linear Regression.
7. Additional analysis : Perform Linear Regression with only one independent variable
    - Extract just the median_income column from the independent variables (from X_train and X_test).
    - Perform Linear Regression to predict housing values based on median_income.
    - Predict output for test dataset using the fitted model.
    - Plot the fitted model for training data as well as for test data to check if the fitted model satisfies the test data.


### Tools used:
This project was completed in Python using Jupyter notebooks.
Common libraries used for analysis include numpy, pandas, matplotlib, seaborn, sklearn
