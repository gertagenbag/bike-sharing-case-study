# Bike Sharing Case Study

## Table of Contents
* [General Info](#general-information)
* [Dataset](#dataset)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
The purpose of this project was to identify the driving factors behind demand for a bike sharing service.  A multiple linear regression model was constructed for the prediction of demand for shared bikes.

The requirements were that the model must be usable by the management of the bike sharing company to understand the drivers of demand.  Such understanding may enable the business to manipulate the business strategy accordingly and to understand the demand dynamics of new markets.  Simplicity and interpretability of the model was thus prioritized over absolute accuracy.

## Dataset
The analyzed dataset was supplied as part of the UpGrad AI&ML programme.  The dataset can be found [here](https://ml-course2-upgrad.s3.amazonaws.com/Linear+Regression+Assignment/Bike+Sharing+Assignment/day.csv).

Summary of the dataset:
- Period: 2018 - 2019
- Number records: 730

## Methodology
Dummy categorical variables were introduced and the dataset was normalized.  The dataset was explored to identify independent variables that had a linear correlation with the target dependant variable.

A linear regression model was trained against 70% of the records in the supplied dataset by iteratively introducing variables one at a time, and then removing variables which had high p-values or drove up the variance inflation factors of other variables.

The model was evaluated for linearity, homoscedasticity, normality, and independence of predictor variables.  Finally, the model was evaluated against the remaining 30% of the records in the supplied dataset.

The final model explains 74.4% of the variance of the predicted variable using only five predicting variables.  The p-values for all predictor variables are very low (<0.001) in this model.  This suggests that the model has very strong statistical significance.

## Conclusions
The following strong driving factors behind bike sharing demand was identified:
- Apparent Temperature: +0.63
- Operational Years: +0.24
- Light Rain or Snow: -0.21
- Wind Speed: -0.14
- Mist: 0.07

## Technologies Used
The following Python libraries were utilized:
- Pandas
- Numpy
- Seaborn
- Matplotlib
- Sklearn
- Scipy
- Statsmodels

## Contact
Created by @gertagenbag
