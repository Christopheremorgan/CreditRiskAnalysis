# CreditRiskAnalysis

## Overview of the analysis: 
Leverage multiple methodologies and techniques to predict credit risk using a credit dataset from the peer-to-peer lending services company, LendingClub. 

Credit risk is an inherently unbalanced classification problem where good loans signficantly outnumber risky loans.  Python imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling algorithms including RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN.

To reduce bias, the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models were used to predict credit risk.  The models are compared the performance of each are evaluated.

## Results: 
Below we compare the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Naive Random Oversampling
- balanced accuracy score: 0.65
- high credit risk precision score: 0.01
- high credit risk recall score: 0.72

[insert confusion matrix]
[insert imabalance classification report]


### SMOTE Oversampling
- balanced accuracy score: 0.66
- high credit risk precision score: 0.01
- high credit risk recall score: 0.64

[insert confusion matrix]
[insert imabalance classification report]


### Cluster Centroid Resampling
- balanced accuracy score: 0.54
- high credit risk precision score: 0.01
- high credit risk recall score: 0.69

[insert confusion matrix]
[insert imabalance classification report]


### SMOTEENN Combinatorial Resampling
- balanced accuracy score: 0.67
- high credit risk precision score: 0.01
- high credit risk recall score: 0.76

[insert confusion matrix]
[insert imabalance classification report]


### Balanced Random Forest Classifier
- balanced accuracy score: 0.77
- high credit risk precision score: 0.03
- high credit risk recall score: 0.68

[insert confusion matrix]
[insert imabalance classification report]


### Easy Ensemble Adaboost Classifier
- balanced accuracy score: 0.93
- high credit risk precision score: 0.09
- high credit risk recall score: 0.92

[insert confusion matrix]
[insert imabalance classification report]


## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

## Code Files
credit_risk_resampling.ipynb
credit_risk_ensemble.ipynb

