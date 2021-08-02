# Credit Risk Analysis

## Overview of Project:
Employ several resampling techniques and machine learning models to predict Credit risk from credit card dataset. Given credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans, employing different techniques to train and evaluate models with unbalanced classes is essential for better prediction of 'high risk' credit.

### Purpose:
Use `imbalanced-learn` and `scikit-learn` libraries to build and evaluate models predicting credit risk using resampling. Followings are the type of resampling we use on the credit card credit dataset from LendingClub:
- oversample the data using the `RandomOverSampler` and `SMOTE` algorithms.
- undersample the data using the `ClusterCentroids` algorithm. 
- combinatorial approach of over- and undersampling using the `SMOTEENN` algorithm. 
- compare two new machine learning models that reduce bias, `BalancedRandomForestClassifier` and `EasyEnsembleClassifier`.

Lastly, we review the performance of each model and evaluate which approach is suited for predicting the credit risk of the given dataset.

### Resources:
- Dataset: 'LoanStats_2019Q1.csv'
- Program: Jupyter Notebook

## Results:
#### Naive Random Oversampling:
+ The accurary score of model is 64.9%. The precision of 'high_risk' credit is as low as 1% and recall is 73%. Note that F1 score is also very low due to low precision.  

   ![](images/1_random_oversampling.png)

#### SMOTE oversampling:
+ The accurary score of model is 65.8%. The precision of 'high_risk' credit is as low as 1% and recall is 63%. Note that F1 score is also very low due to low precision.  

   ![](images/2_SMOTE.png)

#### Cluster Centroids undersampling:
+ The accurary score of model is 54.4%. The precision of 'high_risk' credit is as low as 1% and recall is 69%. Note that F1 score is also very low due to low precision.  
   
   ![](images/3_clustercentroids.png)
   
#### SMOTEENN Combination(over and under) sampling:
+ The accurary score of model is 66.2%. The precision of 'high_risk' credit is as low as 1% and recall is 78%. Note that F1 score is also very low due to low precision.  
   
   ![](images/4_SMOTEENN.png)
   
#### Balanced Random Forest Classifier:
+ The accurary score of model is 77.2%. The precision of 'high_risk' credit is slightly higher at 3% and recall is 78%. Note that F1 score is also very low due to low precision. 

   
   ![](images/5_BalancedRandomForestClassifier.png)
   
#### Easy Ensemble AdaBoost Classifier:
+ The accurary score of model is 93.2% and it is much higher compared to the rest. The precision of 'high_risk' credit is also higher at 9% and recall is 92%. Note that F1 score is also slightly higher at 16%.


   ![](images/6_EasyEnsembleClassifier.png)
   

## Summary:
+ Reviewing the performance of all six models, we can see that some models have better accuracy score and balance in precision and recall scores. Especially, Easy Ensemble AdaBoost Classifier is top at accuracy score of 93.2% and precision of predicting high risk credit of 9%, while the other models have less than 3% in precision. This model also has high recall of 92% and thus the F1 score is 16%, much higher than the rest of five models. 
+ Therefore, in this Credit Card Credit Dataset, Easy Ensemble AdaBoost Classifier performs the best in predicting high risk credit.
