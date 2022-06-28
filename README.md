# Credit-Risk-Analysis

# Overview of the analysis

## Purpose
Applying machine learning to solve a real-world challenge - credit card risk. 

## Strategy and dataset
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I need to employ different techniques to train and evaluate models with unbalanced classes. The credit card dataset is taken from LendingClub, a peer-to-peer lending services company. 

I adopted the following procedure:

    oversample the data using the RandomOverSampler and SMOTE algorithms.
    Undersample the data using the ClusterCentroids algorithm.
    Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
    Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

We will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.
