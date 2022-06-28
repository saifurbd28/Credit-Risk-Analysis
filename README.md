# Credit-Risk-Analysis

# Overview of the analysis

## Purpose
Applying machine learning to solve a real-world challenge - credit card risk. 

## Strategy and dataset
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I need to employ different techniques to train and evaluate models with unbalanced classes by using imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. The credit card credit dataset is taken from LendingClub, a peer-to-peer lending services company. Here, I oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm before applying machine learning algorithms (i.e., logistic regression and randomforest)
