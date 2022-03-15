# Credit_Risk_Analysis
## Overview
LendingClub a fast-lending company wants to use machine learning to predict credit risk and believe this is a quicker and more reliable way. Jill the lead analyst and I worked together to implement this plan. We used Machine Learning and techniques such as resampling and boosting to make the most of the models we created and the data to predict trends to optimize lending. We designed and implemented several algorithms and then evaluated the performance to see how each model predicted the data. 

## Analysis
The loan prediction risk analysis involved importing the necessary tools required such as python, scipy, imbalanced-learn and scikit-learn libraries, evaluating three machine learning models by using resampling to determine which is better at predicting credit risk. 
We used supervised learning to solve a classification problem because classification models are used to predict discrete outcomes such as our target which is credit risk. In our case loan status as either being high or low risk.  The process involves the following, instantiate a model, train it, create predictions, then validate the model.
After reading in my data and cleaning and preparing my data which involved to convert textual data into numerical data for machine learning.  Once data was cleaned and prepared, I then split the data into training and testing sets to be used for each training model. I used the train_test_split module from sklearn and split the data into training and testing sets. Used the stratify argument to make sure data is divided proportionally and the random_state remained consistent at 1 to ensure consistency between each resampling sets. I then had to perform different algorithms to determine which algorithm results in the best performance. 
I used oversampling algorithms, undersampling algorithms and a combination of both. 
For the oversampling of the data I used two different algorithms (Naïve Random and Smote ). 
For the undersampling algorithm I used the Cluster Centroids algorithm.  
Finally, I used a Combination (Over and Under) Sampling algorithm (SMOTEENN). 
For each algorithm test 
*  We resampled the training data and trained the model using the algorithm being used (Naïve, Smote, Cluster Centroids and SMOTEENN). We used a counter to count the number of instances by class to verify they are equal in size and in proportion. 
*  Trained the Logistic regression model with the resampled data and validated the model to      create predictions by calculating the balanced accuracy score to give us a better idea of how well the logistic regression model is able to  predict both classes (low or high risk).
*Created a confusion matrix to give insight into the errors being made by the classifier but also types of errors that are being made.  
* Generated a classification report to measure the quality of predictions from a classification algorithm. Shows how many predictions are True and how many are False.  More specifically, True Positives, False Positives, True negatives, and False Negatives are used to predict the metrics of a classification report for each algorithm.  

Here are the results from each algorithm and explanation of each algorithm I used and why. 
* OVERSAMPLING
	* Naïve Random algorithm: (Balanced Accuracy Score of 64%, Precision score of .01 for high risk and F1 score of .02 for high risk loan status)
	
![Naive](https://user-images.githubusercontent.com/94208810/158230373-c0d4151f-5dcc-4deb-85d7-b70ef9301535.png)

	* Smote algorithm creates a sample from the minority class: (Balanced Accuracy Score of 64%, Precision score of .01 for high risk and F1 score of .02 for high risk loan status)
	
	
![Smote](https://user-images.githubusercontent.com/94208810/158230405-e4dbd1ff-4e99-4308-8a1c-499127faeb37.png)

* UNDERSAMPLING
  	* Cluster Centroids: (Balanced Accuracy Score of 64%, Precision score of .01 for high risk and F1 score of .01 for high risk loan status)
	
  	
  ![ClusterCentroids](https://user-images.githubusercontent.com/94208810/158230427-b38cee4c-49e8-4ba0-90dd-33890554ebb1.png)

 * Combination (Over and Under) 
 
 	* SMOTEENN: ( (Balanced Accuracy Score of 51%, Precision score of .01 for high risk and F1 score of .02 for high risk loan status)
	  
 	
 ![SMOTEEN](https://user-images.githubusercontent.com/94208810/158230460-ea169493-a5a8-4e79-a4e3-95a0ff230bbd.png)


I used Ensemble Classifiers to predict credit risk because it creates a machine learning model that is capable of performing better than individually by using multiple models together. THis will help improve the accuracy and robustness as well as decrecrease the variance of the model and increase the overall perfomance of the model. The final prediction is based on accumulated predictions from each algorithm. 

Trained and compared two different ensemble classifiers 

* Balanced Random Forest Classifier randomly under samples each bootstrap sample to balance it. ( (Balanced Accuracy Score of 79%, Precision score of .04 for high risk and F1 score of .07 for high risk loan status)
	 

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/94208810/158257219-89def98d-4cec-4ef2-9a99-35dc8e4e1fca.png)

* Easy Ensemble Classifier balances data by randomly under sampling. ( (Balanced Accuracy Score of 93%, Precision score of .07 for high risk and F1 score of .14 for high risk loan status)
	

![EasyEnsembleClassifier](https://user-images.githubusercontent.com/94208810/158257274-53f4e88b-e494-4a51-860f-f19d2d8d05d0.png)


## Summary 
LendingClub, a peer-to-peer lending services company presented me with a credit card credit dataset. Using several different machine learning models and algorithms, I was able to predict Credit Risk based on the data and compare them.  
After performing the analysis of credit rish using several algorithms I have come to the consclusion with the results listed above for each algorithm. Most all of the precision scores were low for high risk loans. THe ensemble classifiers showed higher balanced accuracy scores with Easy Ensemble Classifier having a high balanced accuracy score of 93% and looking at the highest F1 Score at .14. I believe that Easy Ensemble AdaBoost model was the best to use in predicting credit risk. 

