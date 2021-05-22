# Credit_Risk_Analysis
Using imbalanced-learn and scikit-learn libraries to build and evaluate machine-learning models predicting credit card risk using resampling. 
# Overview of the analysis: 
Explain the purpose of this analysis.

# Results: 
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of youtputs to support your results.

| y values counts, dataset | y values counts, RandomOverSampler | y values counts, SMOTE
:-------------------------:|:-------------------------:|:---------------------------:
![y.values_counts](Images/y.values_counts.png) | ![y.value_counts_RandomOverSampling](Images/y.value_counts_RandomOverSampling.png) | ![y.value_counts_SMOTE_Oversampling](Images/y.value_counts_SMOTE_Oversampling.png)

| accuracy score and confusion matrix, RandomOverSampler | accuracy score and confusion matrix, SMOTE 
:------------------------:|:---------------------------------:
![RandomOverSampler_score_and_matrix](Images/RandomOverSampler_score_and_matrix.png) | ![SMOTE_score_matrix](Images/SMOTE_score_matrix.png)

| classification report, RandomOverSampler | classification report, SMOTE 
:---------------------:|:---------------------------:
![RandomOverSampler_classification_report](Images/RandomOverSampler_classification_report.png) | ![SMOTE_classification_report](Images/SMOTE_classification_report.png)

| accuracy score and confusion matrix, ClusterCentroids | accuracy score and confusion matrix, SMOTEENN |
:----------------------:|:------------------------------:
![ClusterCentroids_score_matrix](Images/ClusterCentroids_score_matrix.png) | ![SMOTEENN_score_matrix](Images/SMOTEENN_score_matrix.png)

| classification report, ClusterCentroids | classification report, SMOTEENN |
:-------------------------:|:---------------------------------:
![ClusterCentroids_classification_report](Images/ClusterCentroids_classification_report.png) | ![SMOTEENN_classification_report](Images/SMOTEENN_classification_report.png)

| accuracy score and confusion matrix, RandomForest | accuracy score and confusion matrix, EasyEnsemble 
:--------------------------:|:------------------------------------:
![RandomForest_score_matrix](Images/RandomForest_score_matrix.png) | ![EasyEnsemble_score_matrix](Images/EasyEnsemble_score_matrix.png)

| classification report, RandomForest | classification report, EasyEnsemble
:-------------------------------:|:---------------------------:
![RandomForest_classification_report](Images/RandomForest_classification_report.png) | ![EasyEnsemble_classification_report](Images/EasyEnsemble_classification_report.png) 

# Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
