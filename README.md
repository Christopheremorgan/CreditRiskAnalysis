# CreditRiskAnalysis

## Overview of the analysis: 
Multiple methodologies and techniques are leveraged to predict credit risk using a dataset from LendingClub, which is a peer-to-peer lending services company. 

As credit risk is an  unbalanced classification problem where good loans signficantly outnumber risky loans, Python imbalanced-learn and scikit-learn libraries are used to build and evaluate models. Resampling algrotihms include RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN.

To reduce bias, the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models are also used to predict credit risk.  The performance of each model is compared and evaluated.

## Results: 
Below we compare the balanced accuracy scores and the precision and recall scores of all six machine learning models and include images of their confusion matrix and imbalanced classification report. 

### Naive Random Oversampling
- balanced accuracy score: 0.65
- high credit risk precision score: 0.01
- high credit risk recall score: 0.72

![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/ros_cm.png)
![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/ros_icr.png)

### SMOTE Oversampling
- balanced accuracy score: 0.66
- high credit risk precision score: 0.01
- high credit risk recall score: 0.64

![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/smote_cm.png)
![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/smote_icr.png)

### Cluster Centroid Resampling
- balanced accuracy score: 0.54
- high credit risk precision score: 0.01
- high credit risk recall score: 0.69

![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/cc_cm.png)![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/cc_icr.png)

### SMOTEENN Combinatorial Resampling
- balanced accuracy score: 0.67
- high credit risk precision score: 0.01
- high credit risk recall score: 0.76

[insert confusion matrix]
[insert imabalance classification report]
![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/smoteenn_cm.png)![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/smoteenn_icr.png)

### Balanced Random Forest Classifier
- balanced accuracy score: 0.77
- high credit risk precision score: 0.03
- high credit risk recall score: 0.68

![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/brf_cm.png)![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/brf_icr.png)

### Easy Ensemble Adaboost Classifier
- balanced accuracy score: 0.93
- high credit risk precision score: 0.09
- high credit risk recall score: 0.92

![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/eeabc_cm.png)![image_name](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/resources/eeeabc_icr.png)

## Summary: 
The Easy Ensemble Adaboost Classifier algorithm performed significantly higher on all measure of performance when compared to the  other ML algorithms when predicting high credit risk.  As we look at the confusion matrix we find that for every high credit risk we correctly identify we incorrectly identify 10 good loans as high risk loans.  So as long as the avoided risk of bad loan adds more value than the proceeds of 10 good loans this model could be a useful tool to faciliate loan approval.

## Code Files
[credit_risk_resampling.ipynb](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/credit_risk_resampling.ipynb)

[credit_risk_ensemble.ipynb](https://github.com/Christopheremorgan/CreditRiskAnalysis/blob/main/credit_risk_ensemble.ipynb)


