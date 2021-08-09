# CreditRiskAnalysis

## Overview of the analysis: 
Leverage multiple methodologies and techniques to predict credit risk using a credit dataset from the peer-to-peer lending services company, LendingClub. 

Credit risk is an inherently unbalanced classification problem where good loans signficantly outnumber risky loans.  Python imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling algorithms including RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN.

To reduce bias, the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models were used to predict credit risk.  The models are compared the performance of each are evaluated.

## Results: 
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Naive Random Oversampling

### SMOTE Oversampling

### Cluster Centroid Resampling

### SMOTEENN Combinatorial Resampling

### Balanced Random Forest Classifier

### Easy Ensemble Adaboost Classifier


## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

## Code Files
credit_risk_resampling.ipynb
credit_risk_ensemble.ipynb

