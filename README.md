# Credit-Risk-Classification

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

* Machine Learning Model 1:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.98      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384
* The accuracy is high (98.89%)
* Some of the caseses it identified as high-risk may not be truly high-risk (precision = 0.84, wrongly classified = 113 cases) 
* While truly high-risk loans weren't missed a lot (recall = 0.98, wrongly classified = 10 cases)



* Machine Learning Model 2:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.83      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384
* The accuracy is high (99.34%)
* Some of the cases it identified as high-risk may not be truly high-risk (precision = 0.83, wrongly classified = 125 cases) 
* While truly high-risk loans weren't missed a lot (recall = 0.99, wrongly classified = 4 cases)

## Summary

The two models have pretty similar results. If we have to pick, Model 2 might be better in this case for predicting high-risk loans. The high-risk cases it missed to identify are slightly less then Model 1.

The reason being we would want to identify as much high-risk loans as possible, so in this case, higher recall is better.
