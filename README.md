# Module 12 Report Template

## Overview of the Analysis

### Purpose of the analysis:
The purpose of the analysis is to predicted risky loans based on different loan charactaristics

### Data used:
The data we used for the analysis is historical loans information and data which tells if the loan has a high risk of defaulting.

### Variables I was trying to predict
Based on the historical information I was trying to predict if new loans will have a high risk of defaulting

### The Stages of the Machine Learning processing I performed:
I followed the following steps to perform the prediction:
1. Separate the data to train and test
2. Fit a logistics regression model with the training data
3. Evaluate the model results by comparing the model predictions and the labels of the test data
4. Using a random over sampler to resample the training data (in order to increase the proportion of high risk loans in the data)
5. run the logistics regression model with the resampled data
6. Evaluate the resampled model results by comparing the model predictions and the labels of the test data.
7. Compare the results of the two models

## Results

### Machine Learning Model 1:
  - Logistics Regression Model (random state = 1). Using the original features data
  - Accuracy: 95.2%
  - Precision: 100%
  - Recall: 91%

### Machine Learning Model 2:
  - Logistics Regression Model (random state = 1). Using the resampled features data
  - Accuracy: 99.3%
  - Precision: 100%
  - Recall: 99% 


## Summary

Since the loans dataset was imbalanced, it is recommended to perform a resampling on the data before applying a logistics regression model to predict risky and healthy loans. 
While the resampling is less important to predict healthy loans, it is providing much more accuracy for high risk loans predictions