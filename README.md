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

In total, I trained six machine learning models to complete three tasks. The list of the models used under each task is below.

### Resampling Models to Predict Credit Risk
1. Naive Random Oversampling using RandomOverSampler

**Results:** 
* The balanced accuracy score for this model was 66%
* The precision score for high risk individuals was 1% with a recall score of 74%
* The precision score for low risk individuals was 100% with a recall score of 58%
* The overall average precision score was 99% with a recall score of 58%

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/1_RandomOverSampler.PNG)

2. Oversampling using SMOTE

**Results:** 
* The balanced accuracy score for this model was 65%
* The precision score for high risk individuals was 1% with a recall score of 62%
* The precision score for low risk individuals was 100% with a recall score of 68%
* The overall average precision score was 99% with a recall score of 68%

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/2_SMOTE.PNG)

3. Undersampling using ClusterCentroids

**Results:** 
* The balanced accuracy score for this model was 59%
* The precision score for high risk individuals was 1% with a recall score of 64%
* The precision score for low risk individuals was 100% with a recall score of 53%
* The overall average precision score was 99% with a recall score of 53%

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/3_ClusterCentroids.PNG)

### SMOTEENN Algorithm to Predict Credit Risk
1. Combinatorial using SMOTEEN

**Results:** 
* The balanced accuracy score for this model was 64%
* The precision score for high risk individuals was 1% with a recall score of 72%
* The precision score for low risk individuals was 100% with a recall score of 57%
* The overall average precision score was 99% with a recall score of 57%

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/4_SMOTEEN.PNG)

### Ensemble Classifiers to Predict Credit Risk
1. Balanced Random Forest Classifier using BalancedRandomForestClassifier

**Results:** 
* The balanced accuracy score for this model was 78%
* The precision score for high risk individuals was 3% with a recall score of 57%
* The precision score for low risk individuals was 100% with a recall score of 88%
* The overall average precision score was 99% with a recall score of 88%

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/5_BalancedRandomForestClassifier.PNG)

2. Easy Ensemble AdaBoost Classifier using EasyEnsembleClassifier

**Results:** 
* The balanced accuracy score for this model was 92%
* The precision score for high risk individuals was 9% with a recall score of 89%
* The precision score for low risk individuals was 100% with a recall score of 94%
* The overall average precision score was 99% with a recall score of 94%

![image](https://github.com/dwwatson1/Credit_Risk_Analysis/blob/main/Images/6_EasyEnsembleClassifier.PNG)

## Summary of the Results

### Summary

### Model Recommendation


