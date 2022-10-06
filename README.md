# Cardiovascular-Risk-Prediction--Viral-Shewale

## Abstract:
* Cardiovascular disease (CVD) is a group of disorders of the heart and blood vessels and includes coronary heart disease, cerebrovascular disease, rheumatic heart disease and other conditions.
* Cardiovascular diseases (CVDs) are the leading cause of death globally, taking an estimated 17.9 million lives each year.
* Though CVDs cannot be treated, predicting the risk of the disease and taking the necessary precautions and medications can help to avoid severe symptoms and, in some cases, even death.

## Problem Statement: 
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD).


## Model selection approach:

* We are working on a binary classification problem.
* Here we can start with a simple model, as a baseline model, which is interpretable, ie. Logistic Regression.
* Try other standard binary classification models like Naive Bayes, decision tree classifiers, and support vector machines.
* Use ensemble models with hyperparameter tuning to check whether they give better predictions.

## Evaluation metrics:

* Since the data we are dealing with is unbalanced, accuracy may not be the best evaluation metric to evaluate the model performance.
* Also, since we are dealing with data related to healthcare, False Negatives are big concern than False Positives.
* In other words, it doesn’t matter whether we raise a false alarm, but the actual positive cases should not go undetected. After considering all the above points. The recall score would be the best evaluation metric.
* **Recall = TruePositives / (TruePositives + FalseNegatives)**


## Conclusion:

* I trained 6 Machine Learning models using the training dataset with hyperparameter tuning to improve the model performance.
* The dataset contained some null values, outliers and also data were unbalanced. Unbalance data were handled using SMOTE to reduce bias on one outcome.
* The Recall was chosen as the model evaluation metric because it doesn’t matter whether we raise a false alarm, but the actual positive cases should not go undetected. 
* The initial set of predictions obtained using the baseline model, i.e. logistic regression model, and other commonly used classification models was also built in search of better predictions.
* The model I developed must have a high recall score. It is ok if the model incorrectly identifies a healthy patient as a high-risk patient because this would not lead to death, but if the high-risk patient was incorrectly labelled as healthy, it could result in fatality.
* We were able to create a model with a recall of just 0.80 because of limited data available and limited computational power available.
* A recall score of 0.80 indicates that out of 100 individuals with the illness, our model will be able to classify only 80 as high-risk patients, while the remaining 20 will be misclassified.
* From the analysis, I found that the age of a person was the most important feature in determining the risk of a patient getting infected with CHD, followed by pulse pressure, prevalent hypertension and total cholesterol.
* Diabetes, prevalent stroke and BP medication were the least important features in determining the risk of CHD.
