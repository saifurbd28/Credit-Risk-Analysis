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

# Deliverable 1: Use Resampling Models to Predict Credit Risk

## Oversampling models

### Model-1: Naive Random Oversampling
![Model-1](https://user-images.githubusercontent.com/100442163/176254360-eb6c06e7-6d7d-4679-9364-d440a2f224b3.png)

The balanced accuracy score is 66%.
The high_risk precision is very low (1% only) with 72% precision and 60% specificity which makes a F1 of 2% only.
On the other hand, the low_risk precision is 100% with 60% precision and 72% specificity. It gives a F1 value of 75%.
This high precision of the low_risk credit is due to the high number of the low_risk population. 


### Model-2: SMOTE Oversampling

![Model-2](https://user-images.githubusercontent.com/100442163/176255320-a5ef5707-0027-48bb-83e6-53e1186ab401.png)

A similar result can be observed here. The balanced accuracy score is 65.7%. Other scores are also similar. 

## Undersampling model

### Model-3: Cluster Centroids for Undersampling

![Model-3](https://user-images.githubusercontent.com/100442163/176255328-fd426184-ccf6-4a14-aa58-19a2c0455f9d.png)

Here the balanced accuracy score is down to about 54%.
The high_risk precision is still 1% only with 69% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 40%. 

# Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk

## Combination (Over and Under) Sampling

## Model-4: Combination (Over and Under) Sampling using the SMOTEENN algorithm
![Model-4](https://user-images.githubusercontent.com/100442163/176256056-13d53be2-c89c-459a-8734-8cfc3c103ced.png)

The balanced accuracy score is about 54%.
The high_risk precision is still 1% only with 69% sensitivity which makes a F1 of only 1%.
Due to the high number of false positives, the low_risk sensitivity is 40%. 

# Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

## Model-5: Balanced Random Forest Classifier
![Model-5](https://user-images.githubusercontent.com/100442163/176256569-8aae6daf-01ee-421e-8ea5-d472021c5518.png)
The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

## Model-6: Easy Ensemble AdaBoost Classifier

![Model-6](https://user-images.githubusercontent.com/100442163/176256856-1ec9d491-d49b-450b-b1af-2a85b25de123.png)

Now, the balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion. 

# Summary
The performace of all these models to predict the high credit risk were poor. It is due to lower population size in this category. So, models were failed to get proper training. It suggest that population size is very important in proper model training. On the other hand, all models had a relatively better predictive score for low credit risk group. It is due to the trained data was mainly the data of low risk population. 







