# Credit Risk Classification Analysis

## Overview

The purpose of this analysis was to generate a machine learning model for the purpose of classifying credit loans as Healthy or High Risk of Defaulting. Financial information such as loan size, interest rate, income, debt to income, number of accounts, and derogatory marks are the criteria used to evaluate the loan status.


Key steps in the machine learning process included:

- Data preprocessing and feature selection (establishing X and y variables)
- Splitting the dataset into training and testing sets.
- Training a logistic regression model and evaluating its performance using key metrics such as accuracy, precision, and recall.
- Interpreting results and making recommendations based on model performance.

## Results

- Confusion Matrix:
- - True Positive: 18658
- - False Positive: 37
- - False Negative: 107
- - True Negative: 582


- Classification Report:
- - Precision:
- - - Healthy: 1.00
- - - High-Risk Loan: 0.84
- - Recall:
- - - Healthy: 0.99
- - - High-Risk Loan: 0.94
- - F1-score:
- - - Healthy: 1.00
- - - High-Risk Loan: 0.89
- - Accuracy: 0.99
- - Macro Avg: 0.92 (Precision), 0.97 (Recall), 0.94 (F1-score)
- - Weighted Avg: 0.99 (Precision), 0.99 (Recall), 0.99 (F1-score)

## Summary

The logistic regression model performed exceptionally well with an accuracy of 99%. The model has a recall percentage of correctly classifying High-Risk loans at 94%. This means of all high-risk loans, the model will detect 94%, which is an impressive number. However, the model's High-Risk precision score is 84%, which means the model will misclassify more Healthy loans as high-risk.


## Recommendation

The logistic regression model is a strong candidate for deployment, particularly if recall is prioritized over precision. If the business objective is to minimize the risk of approving high-risk loans, this model is suitable. However, if false positives (misclassifying healthy loans as high-risk) pose a significant concern, alternative models may be explored.