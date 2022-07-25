# Credit_Risk_Analysis
Employ different techniques to train and evaluate ML models.

## Overview 
Using a credit card dataset from LendingClub different techniques were employed to understand credit risk.  The initial technique used was to oversample the data using the RandomOverSampler, then SMOTE algorithms, followed by a undersample to the data using the ClusterCentroids algorithm. Last a combinatorial approach of over and undersampling using the SMOTEENN algorithm was used.

Additionally, two more machine learning models were made that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.  These modes were then compared against each other on how well they do to predict credit risk. The evaluation of the performance of these models was necessary to understand if they should be used a predictive tool.


Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

## Libraries and ML Models

1. imblearn 
2. sklearn
3. RandomOverSampler
4. SMOTE
5. BalancedRandomForestClassifier
8. EasyEnsembleClassifier

## ML Results
A total of six machine learning models were created.  The models all varied in their accuracy, precision and recall.  Below are the main examples:

### Naive Random Oversampling
![NR](https://github.com/vhernandezjr/Credit_Risk_Analysis/blob/main/PNG/NaiveRandom.png)     
1. Balanced Accuracy: 0.6409687725362696
2. Recall: High/Low risk = .61/.67

### SMOTE Oversampling
![SO](https://github.com/vhernandezjr/Credit_Risk_Analysis/blob/main/PNG/SMOTE.png)     
1. Balanced Accuracy: 0.6248967612233141
2. Recall: High/Low risk = .62/.63

### Undersampling
![US](https://github.com/vhernandezjr/Credit_Risk_Analysis/blob/main/PNG/Undersampling.png)     
1. Balanced Accuracy: 0.6248967612233141
2. Recall: High/Low risk = .57/.45

### Combination Over and Under Sampling
![COU](https://github.com/vhernandezjr/Credit_Risk_Analysis/blob/main/PNG/O_U_Sampleing.png)     
1. Balanced Accuracy: 0.5127331181937947
2. Recall: High/Low risk = .70/.58

### Balanced Random Forest Classifier
![RF](https://github.com/vhernandezjr/Credit_Risk_Analysis/blob/main/PNG/Balanced%20RF.png)     
1. Balanced Accuracy: 0.7877672625306695
2. Recall: High/Low risk = .67/.91

### Easy Ensemble AdaBoost Classifier
![EEAB](https://github.com/vhernandezjr/Credit_Risk_Analysis/blob/main/PNG/E_Ensemble_AdaBoost.png)     
1. Balanced Accuracy: 0.925427358175101
2. Recall: High/Low risk = .91/.94

## Summary

The best-balanced accuracy score for a machine learning model sits closer to 1 when looking at the 0 – 1 scale.  Out of the models run in this exercise, the Easy Ensemble AdaBoost Classifier scored the best with a .925 balanced accuracy.  For this particular data set we found that all models did well but the EEAC model was best.
