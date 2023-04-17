# UCB-Project-3
Exploring ML models to predict if the bank client opens term deposit account.


THE GOAL

The goal is to find the best ML model for predicting the term deposit account opening by using the bank data client's characteristics as features.

THE DATA

Data represents 17 Portuguese bank campaigns that occurred between May 2008 and November 2010, corresponding to a total of 79354 contacts.

THE FILES

This project consists of 3 notebooks:
* Main_notebook_unbalanced_data
* Support_notebook_ 1_balanced_oversampled
* Support_notebook_ 2_balanced_undersampled

The Main notebook explores the models with unbalanced data while the other two are based on balanced data by using oversampling/undersampling techniques.

Data file is also included.


RESULTS

After exploring the dataset with balanced and unbalanced data and running many models (only few included in the three notebooks) I discovered that even though most models had very high accuracy the other parameters (Precision, Recall, F1 score) were very poor and with AUC hovering between 50% - 59% models resembled a random chance. That led me to deeper exploration of values used for creating the model and it turned out that all of the values are having similar proportions for opening and not opening the term deposit account. Hence we can't get a usable ML model because none of the values show enough difference to create a ML model. In order to create a model we would need to explore other features from the original data set. Hopefully other features may contain more useful information for predicting the term deposit account opening. Another option would be to keep increasing the data collection until the pattern emerges. 
