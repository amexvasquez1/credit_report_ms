# Module 12 Report Analysis

![](Images/loan.png)

## Overview of the Analysis

In this Credit Risk Classification challenge, we reviewed a set of lending data and used different techniques to train machine learning models to identify high-risk loans from the data to minimize risk.

The variables provided in the lending data file are features such as loan size, interest rate, borrower income, debt to income ratio, etc. There are a total of 75036 entries of healthy loans, and 2500 high-risk loans in the data set.

To analyze the data, we did the following steps:

* Read csv file and review data frame.
* Fit the model
* Make predictions
* Evaluate the model with Confusion Matrix
* Generate classification report

Initially we used Logistic Regression model without over or undersampling the dataset. After reviewing the first set of classification report, we conducted a new around with RandomOverSampler module, repeated all the steps 2-5. Compared both sets of the classification report to determine which module gives better prediction..

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models.

* Machine Learning Model 1:
  * Logistic Regression Model with Original Data ("0": healthy loan, "1": high-risk loan) Balanced Accuracy Score = 0.95 Precision "0" = 0.99 Precision "1" = 0.91 Recall "0" = 1.00 Recall "1" = 0.85



* Machine Learning Model 2:
  * Logistic Regression Model with Oversampled Data ("0": healthy loan, "1": high-risk loan) Balanced Accuracy Score = 0.99 Precision "0" = 1.00 Precision "1" = 0.84 Recall "0" = 0.99 Recall "1" = 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Per my obervation based on the type of data that we received I would suggest using the Logistic Regression Model with Oversampled Data whcih gives an improved accuracy score at 0.99 from 0.95; and also enhanced Recall value for high-risk loans from 0.85 to 0.99.
