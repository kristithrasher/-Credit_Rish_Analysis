# Credit_Risk_Analysis
## Overview
Used Machine Learning to solve a real-world challenge credit card risk. LendingClub, a peer-to-peer lending services company presented me with a credit card credit dataset. Using different Models to predict Credit Risk and compare them and decide if there is one with positive performace that I would reccomend a model to predict credit risk. 

## Analysis
The loan prediction risk analysis involved importing the necessary tools required such as imbalanced-learn and scikit-learn libraries, evaluating three machine learning models by using resampling to determine which is better at predicting credit risk. I used oversampling algorithms, undersampling algorithms and a combination of both.
First, I oversampled the data using two different algorithms (Naïve Random Oversampling, Smote Oversampling). I then tested a undersampling algorithm (Cluster Centroids algorithm) to determine which algorithm results in the best performance compared to the oversampling algorithms.  Finally, I used a Combination (Over and Under) Sampling algorithm (SMOTEENN algorithm) to determine if the algorithm results in the best performance by comparing those to the other sampling algorithms. For each algorithm test I viewed the count of the target classes, resampled the data and trained it using the logistic regression model, calculated the balanced accuracy score, printed the confusion matrix and generated a classification report for each algorithm. 
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
