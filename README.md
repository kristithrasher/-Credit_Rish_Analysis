# Credit_Risk_Analysis
## Overview
LendingClub, a peer-to-peer lending services company presented me with a credit card credit dataset. Using different Models to predict Credit Risk and compare them and decide if there is one with positive performace that I would reccomend a model to predict credit risk. 

## Analysis
Compared two oversampling algorithms to determine which algorithm results in the best performance. I oversampled the data using two different algorithms (Naïve Random Oversampling, Smote Oversampling). I then tested a undersampling algorithm (Cluster Centroids algorithm) to determine which algorithm results in the best performance compared to the oversampling algorithms.  I also used a Combination (Over and Under) Sampling algorithm (SMOTEENN algorithm) to determine if the algorithm results in the best performance by comparing those to the other sampling algorithms. SO for each algorithm test I viewed the count of the target classes, resampled the data and trained it using the logistic regression model, calculated the balanced accuracy score, printed the confusion matrix and generated a classification report for each algorithm. 
Here are the results from each algorithm

* OVERSAMPLING
	* Naïve Random 
	* Smote 

* UNDERSAMPLING
  	* Cluster Centroids
 	 * Combination (Over and Under) SMOTEENN  

I used Ensemble Classifiers to Predict Credit Risk
Trained and compared two different ensemble classifiers by resampling the dataset, checked the count of the target classes to make sure they were equal and trained the ensemble classifier to calculate the balanced accuracy score, generate a confusion matrix and generate a classification report. 
* BalanceRandomForestClassifier

* EasyEnsembleClassifier


## Summary 
* Results
* Recommendation on which model  to use or there is no recommenmdatiomn with a justification. 
