# Bike Sharing Assignment


## Table of Contents
* [General Info](#general-information)
* [Contents](#contents)
* [Technologies Used](#technologies-used)
* [Steps performed](#Steps-performed)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- This repository contains the code for Linear Regression modeling on Bike sharing dataset.
- Problem Statement: A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free.
A US bike-sharing provider BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19.
They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.
The company wants to know:
Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands

- Dataset used: day.csv

## Contents
- Notebook: EPGPML58_AnishVA_BikeSharing.ipynb
- Document: Linear_Regression_Subjective_Questions.pdf

## Steps Performed
Following steps were perfomed to create the model and do the prediction
- Reading and Understanding the Data
- Data cleaning (missing value, data duplicate check etc.)
- Dropping irrelavant feature columns based on initial data understanding
- Visualising the Data
- Data Preparation (Creating dummy varaibles for categorical columns)
- Splitting the Data into Training and Testing Sets
- Rescaling the Features (Using Min-Max scalar)
- Dividing tarin data into X and Y sets for the model building
- Building the model (Model shall be built using LinearRegression function from SciKit Learn for its compatibility with RFE (which is a utility from sklearn))
- Building model using statsmodel (OLS), for the detailed statistics
- Calculate VIF for multicollinearity check
- Residual Analysis of the train data
- Making Predictions with test data (Applying the scaling on the test sets, Dividing into X_test and y_test, predict with x_test data)
- Model Evaluation (# Plotting y_test and y_pred to understand the spread, calculate R2, Adjusted R2 for test data)


## Conclusions
Based on the model metrics, here are the inferences.
- Top 3 features contributing significantly towards explaining the demand of the shared bikes are:
    Temp (Temperature): It has coefficient of  0.509903
    Yr (year): It has coefficient of 0.232930
    Weathersit_3 (Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds): It has coefficient of  -0.294243
- From the distplot of residuals it is observed that Error terms are normally distributed with mean zero
- Based on the R2 and Adjusted-R2 values, the model apperas to be performing well on both training and test data

For more details, refer to EPGPML58_AnishVA_BikeSharing.ipynb


## Technologies Used
- Seaborn version: 0.12.2
- Matplotlib version: 3.7.0
- Python version: 3.10.9
- scikit-learn version: 1.2.1
- statsmodels version: 0.13.5



## Contact
Created by [@anishnairva] - feel free to contact me!
