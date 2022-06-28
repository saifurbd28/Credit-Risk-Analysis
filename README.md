# Credit-Risk-Analysis

# Overview of the analysis

## Purpose
Applying machine learning to solve a real-world challenge - credit card risk. 

## Strategy and dataset
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I need to employ different techniques to train and evaluate models with unbalanced classes. The credit card dataset is taken from LendingClub, a peer-to-peer lending services company. 

I adopted the following procedure:
1) oversample the data using the RandomOverSampler and SMOTE algorithms.
2) Undersample the data using the ClusterCentroids algorithm.
3) Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
4) Compare machine learning models (i.e., logistic regression, Balanced Random Forest Classifier, and Easy Ensemble AdaBoost Classifier).

After evaluating the performance of these models I will make a recommendation on whether they should be used to predict credit risk.

# Results 

## Deliverable 1: Use Resampling Models to Predict Credit Risk

## Model-1: Naive Random Oversampling
![Model-1](https://user-images.githubusercontent.com/100442163/176254360-eb6c06e7-6d7d-4679-9364-d440a2f224b3.png)

## Model-2: SMOTE Oversampling

![Model-2](https://user-images.githubusercontent.com/100442163/176255320-a5ef5707-0027-48bb-83e6-53e1186ab401.png)

## Model-3: Cluster Centroids for Undersampling

![Model-3](https://user-images.githubusercontent.com/100442163/176255328-fd426184-ccf6-4a14-aa58-19a2c0455f9d.png)
