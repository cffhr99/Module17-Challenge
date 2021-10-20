# Module17-Challenge:Credit Risk Analysis
## Overview:
The project used the credit card credit dataset from LendingClub, a peer-to-peer lending services company. RandomOverSampler and SMOTE algorithms were used to oversample the data and ClusterCentroids algorithm was used to undersample the data. Furthermore, a combinatorial approach of over- and undersampling used the SMOTEENN algorithm. Next, BalancedRandomForestClassifier and EasyEnsembleClassifier were compared two new machine learning models that reduce bias to predict credit risk.
## Results:
### credit_risk_resampling.ipynb
#### Logistic Regression with different resampling:
##### Naive Random Oversampling:
  - Balanced Accuracy Score: 64.5%. 
  - High Risk Precision:0.01
  - High Risk Recall: 0.61
  - Low Risk Precision: 1.00
  - Low Risk Recall: 0.68
##### SMOTE Oversampling:
  - Balanced Accuracy Score: 62.9%. 
  - High Risk Precision:0.01
  - High Risk Recall: 0.63
  - Low Risk Precision: 1.00
  - Low Risk Recall: 0.63
##### Cluster Centroid Undersampling:
  - Balanced Accuracy Score: 52.0%. 
  - High Risk Precision:0.01
  - High Risk Recall: 0.60
  - Low Risk Precision: 1.00
  - Low Risk Recall: 0.44
##### SMOTEENN Combination (Over and Under) Sampling:
  - Balanced Accuracy Score: 63.9%. 
  - High Risk Precision:0.01
  - High Risk Recall: 0.69
  - Low Risk Precision: 1.00
  - Low Risk Recall: 0.59
### credit_risk_ensemble.ipynb
##### Balanced Random Forest Classifier:
  - Balanced Accuracy Score: 73.4%. 
  - High Risk Precision:0.02
  - High Risk Recall: 0.60
  - Low Risk Precision: 1.00
  - Low Risk Recall: 0.87
##### Easy Ensemble AdaBoost Classifier: 
  - Balanced Accuracy Score: 92.6%. 
  - High Risk Precision:0.08
  - High Risk Recall: 0.91
  - Low Risk Precision: 1.00
  - Low Risk Recall: 0.94

## Summary:
According to the results of six models above, the easy ensemble adaboost classifier to yield the best metrics for classification of high risk and low risk loan application. Both easy ensemble adaboost classifier and balanced random forest classifier performed significantly better than logistic models with resampling techniques. Among these four resampling methods on logistic models, there is no significant improvement between them.
