# Credit Risk Analysis

## Overview of the Analysis

Determining an individual's credit risk can be challenging because of its inherently unbalanced classification problem. Good loans tend to outnumber risky loans. In this analysis I used different techniques to train and evaluate machine learning models with unbalanced classes. Using imbalanced-learn and scikit-learn libraries, I built and evaluated those models using resampling.

This analysis was completed using six machine learning models beginning with the following. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Next, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Then, I compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once I completed these three parts, I evaluated the performance of these models in the conclusion and made my recommendation on whether they should be used to predict credit risk.

### Analysis Resources
* **Data Sources:** 
  * [LoanStats_2019Q1.csv](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Resources.zip) 
* **Notebooks** 
  * [Credit Risk Ensemble](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Notebooks/credit_risk_ensemble.ipynb)
  * [Credit Risk Resampling](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Notebooks/credit_risk_resampling.ipynb)
* **Software:** Jupyter Notebook 6.1.4, Python 3.7.6, NumPy 1.20.1, SciPy 1.6.2, Scikit-learn 0.24.1

## Results of the Analysis

In total, we trained six machine learning models to complete three tasks. The list of the models used under each task is below.

### Resampling Models to Predict Credit Risk
1. Naive Random Oversampling using RandomOverSampler

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/1_RandomOverSampler.PNG)

2. Oversampling using SMOTE



3. Undersampling using ClusterCentroids

### SMOTEENN Algorithm to Predict Credit Risk
1. Combinatorial using SMOTEEN


### Ensemble Classifiers to Predict Credit Risk
1. Balanced Random Forest Classifier using BalancedRandomForestClassifier



2. Easy Ensemble AdaBoost Classifier using EasyEnsembleClassifier

## Summary of the Results

### Summary

### Model Recommendation


