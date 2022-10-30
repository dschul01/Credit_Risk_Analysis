# Credit_Risk_Analysis

Utilize Python and the SciKit-learn library to build and evaluate machine learning models to predict credit risk.

## Purpose

The purpose of this project is to utilize Python for building multiple machine learning models to predict credit risk.  A credit dataset from a peer-to-peer lending services company is provided as the input for four algorithms and two classifiers to evaluate the performance of the various models.  The results are analyzed to provide a recommendation on which, if any, model should be used to predict risk. 


## Results

The models were developed to predict whether credit applicants should be categorized as high risk (positive cases) compared to low risk (negative cases) depending on a number of features.  The performance of the six machine learning models are explained below including screenshots of each model's output:

<img src="https://github.com/dschul01/Credit_Risk_Analysis/blob/main/Images/Naive_Random_Oversampling.png" width="600" height="250">

* Naive Random Over-Sampling Results
	- Scores: balanced accuracy score = 0.65; precision score = 0.01; recall score = 0.68
	- Performance Overview: The balanced accuracy and recall scores are considered 'ok'. However the model produces an extremely low precision score indicating a substantial volume of false positives.  This model predicted a significant volume of low risk applicants as high risk. 

---------------------------------------------------------------------------------------------------------------------------------
	 
<img src="https://github.com/dschul01/Credit_Risk_Analysis/blob/main/Images/SMOTE_Oversampling.png" width="600" height="250">

* SMOTE Over-Sampling Results
	- Scores: balanced accuracy score = 0.66; precision score = 0.01; recall score = 0.64
	- Performance Overview: The balanced accuracy and recall scores are considered 'ok'. However the model produces an extremely low precision score indicating a substantial volume of false positives.  This model predicted a significant volume of low risk applicants as high risk.

---------------------------------------------------------------------------------------------------------------------------------

<img src="https://github.com/dschul01/Credit_Risk_Analysis/blob/main/Images/Undersampling.png" width="600" height="250">

* Cluster Centroids Under-Sampling Results
	- Scores: balanced accuracy score = 0.54; precision score = 0.01; recall score = 0.69
	- Performance Overview: The balanced accuracy score is considered 'bad' below 60% while the recall score is considered 'ok'. However the model produces an extremely low precision score indicating a substantial volume of false positives.  This model predicted a significant volume of low risk applicants as high risk.

---------------------------------------------------------------------------------------------------------------------------------

<img src="https://github.com/dschul01/Credit_Risk_Analysis/blob/main/Images/Combination_Sampling.png" width="600" height="250">

* SMOTEEN Combination-Sampling Results
	- Scores: balanced accuracy score = 0.67; precision score = 0.01; recall score = 0.79
	- Performance Overview: he balanced accuracy and recall scores are considered 'ok'.  However the model produces an extremely low precision score indicating a substantial volume of false positives.  This model predicted a significant volume of low risk applicants as high risk.

---------------------------------------------------------------------------------------------------------------------------------

<img src="https://github.com/dschul01/Credit_Risk_Analysis/blob/main/Images/Balanced_Random_Forest_Classifier.png" width="600" height="250">

* Balanced Random Forest Classifier Results
	- Scores: balanced accuracy score = 0.79; precision score = 0.03; recall score = 0.70
	- Performance Overview:  The balanced accuracy and recall scores are considered 'ok'. However the model produces an extremely low precision score indicating a substantial volume of false positives.  This model predicted a significant volume of low risk applicants as high risk.

---------------------------------------------------------------------------------------------------------------------------------

<img src="https://github.com/dschul01/Credit_Risk_Analysis/blob/main/Images/Easy_Ensemble_AdaBoost_Classifier.png" width="600" height="250">

* Easy Ensemble AdaBoost Classifier Results
	- Scores: balanced accuracy score = 0.93; precision score = 0.09; recall score = 0.92
	- Performance Overview:  The balanced accuracy and recall scores are considered 'good', but the model produces a low precision score indicating a substantial volume of false positives.  Although the precision score is higher than all other models, there is still a number of low risk applicants predicted as high risk.

---------------------------------------------------------------------------------------------------------------------------------

## Summary

The results above show each machine learning model returned with similiar outcomes of extremely low precision scores.  Low precision scores indicate false positives, so in this case low risk consumers were predicted to be high risk.  Although the AdaBoost Classifier returned with the highest precision score, 6% of applicants would have been treated as high risk and looked at alternative options for their credit needs.  I would not recommend any of these models as I believe false positives should be closer to 1% in determining credit risk.


