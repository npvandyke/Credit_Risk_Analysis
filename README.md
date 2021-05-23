# Credit_Risk_Analysis

Using Python imbalanced-learn and scikit-learn libraries to build and evaluate six different machine-learning models at predicting credit card risk, using resampling and ensemble techniques. 

# Overview of the analysis: 

I've evaluated several different supervised machine-learning models for predicting credit risk using the credit card credit dataset from LendingClub, a a peer-to-peer lending services company. Given the imbalanced nature of the credit card credit dataset, with bad loan applications unsurprisingly accounting for a small percentage of the outcomes (in this case 347 out of 68,817 total outcomes), the first four models involve oversampling, undersampling and combination techniques. These techniques adjust the class distribution of the two potential outcomes in the training datasets of the models in order to influence the fit and reduce bias toward the majority class. The distribution of the testing dataset remains random in order to evaluate the performance of the model. The last two models involve ensemble learning techniques, which combine multiple "weak learning" models to improve the accuracy and robustness of the model while avoiding overfitting. The anticipated outcome is that at least one of these models will be sufficient at predicting bad loan applications despite the underrepresentation of bad loan application outcomes in the given dataset. 

# Results: 

The image below is a key to the confusion matrices which will be discussed in the results for each of the following six machine-learning models. In each of the confusion matrices, the numbers listed from top left to bottom right will indicate the diagnostic results "True Positive", "False Negative", "False Positive" and "True Negative" respectively. 

![Confusion Matrix Key](Images/confusion_matrix_key.png)

The first two machine learning models, RandomOverSampler and SMOTE, used oversampling techniques to resample the minority class. In both models the "low risk" and "high risk" outcomes were evened out in the training dataset to account for 51,352 occurences each. 

*** Discussion of accuracy score and confusion matrix ***

| accuracy score and confusion matrix, RandomOverSampler | accuracy score and confusion matrix, SMOTE 
:------------------------:|:---------------------------------:
![RandomOverSampler_score_and_matrix](Images/RandomOverSampler_score_and_matrix.png) | ![SMOTE_score_matrix](Images/SMOTE_score_matrix.png)

*** Discussion of classification report *** 

| classification report, RandomOverSampler | classification report, SMOTE 
:---------------------:|:---------------------------:
![RandomOverSampler_classification_report](Images/RandomOverSampler_classification_report.png) | ![SMOTE_classification_report](Images/SMOTE_classification_report.png)

The second two machine learning models, ClusterCentroids and SMOTEENN, used undersampling and combination sampling techniques respectively, to...
In ClusterCentroids, the "low risk" and "high risk" outcomes were evened out in the training dataset to 260 occurences each, making for a relatively small training dataset. In SMOTEENN, the "low risk" and "high risk" outcomes were evened out in the training dataset to 46,389 and 51,351 occurences respectively. 

*** Discussion of accuracy score and confusion matrix *** 

| accuracy score and confusion matrix, ClusterCentroids | accuracy score and confusion matrix, SMOTEENN |
:----------------------:|:------------------------------:
![ClusterCentroids_score_matrix](Images/ClusterCentroids_score_matrix.png) | ![SMOTEENN_score_matrix](Images/SMOTEENN_score_matrix.png)

*** Discussion of classification report *** 

| classification report, ClusterCentroids | classification report, SMOTEENN |
:-------------------------:|:---------------------------------:
![ClusterCentroids_classification_report](Images/ClusterCentroids_classification_report.png) | ![SMOTEENN_classification_report](Images/SMOTEENN_classification_report.png)

The final two machine-learning models, RandomForest and EasyEnsemble, used ensemble learning techniques to combine multiple "weak learning" models in order to.... 

*** Discussion of accuracy score and confusion matrix **** 

| accuracy score and confusion matrix, RandomForest | accuracy score and confusion matrix, EasyEnsemble 
:--------------------------:|:------------------------------------:
![RandomForest_score_matrix](Images/RandomForest_score_matrix.png) | ![EasyEnsemble_score_matrix](Images/EasyEnsemble_score_matrix.png)

*** Discussion of classification report **** 

| classification report, RandomForest | classification report, EasyEnsemble
:-------------------------------:|:---------------------------:
![RandomForest_classification_report](Images/RandomForest_classification_report.png) | ![EasyEnsemble_classification_report](Images/EasyEnsemble_classification_report.png) 

# Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

What type of assessment if best for fraud prediction? Why? Which model had the best score for this? 
