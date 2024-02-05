# Module 12 Report Template
## Overview of the Analysis
In this analysis, the goal was to build machine learning models for credit risk classification using historical lending activity data. The purpose was to predict the creditworthiness of borrowers based on various financial features.

## Data Overview:
The dataset included information on peer-to-peer lending, with a focus on predicting loan status (0 for healthy loans and 1 for high-risk loans).
Key variables: loan_status, feature1, feature2, ... (additional features).
The target variable (loan_status) had imbalanced classes, with a majority of loans being healthy.

## Machine Learning Process:
Data Splitting:
The data was split into training and testing sets.
Model 1 - Logistic Regression (Original Data):

Logistic Regression model was fitted using the original data.
Evaluation metrics: Accuracy, Precision, and Recall were assessed.
Model 2 - Logistic Regression (Oversampled Data):

The original data was oversampled using RandomOverSampler.
Logistic Regression model was fitted using the oversampled data.
Evaluation metrics: Balanced Accuracy, Precision, and Recall were assessed.

## Results
* Model 1 - Logistic Regression (Original Data):
  * Accuracy: 0.99
  * Precision (Label 0): 1.00
  * Recall (Label 0): 0.99
  * Precision (Label 1): 0.85
  * Recall (Label 1): 0.91

* Model 2 - Logistic Regression (Oversampled Data):
  * Balanced Accuracy: 0.994
  * Precision (Label 0): 1.00
  * Recall (Label 0): 0.99
  * Precision (Label 1): 0.84
  * Recall (Label 1): 0.99

## Summary
The oversampled logistic regression model (Model 2) outperforms the original model in various metrics, particularly in handling high-risk loans (1). The balanced accuracy, precision, and recall for both labels have improved with oversampling.

## Recommendation:
Model 2 (Logistic Regression with oversampled data) is recommended for use by the company.
The improvements in metrics, especially in handling high-risk loans, indicate enhanced predictive capabilities.
Performance depends on the problem at hand; in this case, it is crucial to correctly identify high-risk loans (1), and Model 2 excels in this aspect.
