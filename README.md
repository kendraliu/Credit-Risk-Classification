# Credit-Risk-Classification

## Overview of the Analysis

This project trains and evaluates a model based on loan risk to identify the creditworthiness of borrowers, using a dataset of historical lending activity from a peer-to-peer lending services company.

A logistic regression model is used to classify each loan into healthy loans (loan status = 0) or high-risk loans (loan status = 1). 

Model 1 and Model 2 are only different in that Model 2 oversamples the training data, for the classes (0/1) are imbalanced in the dataset.


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
