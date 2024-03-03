# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis is to create a module to predict what loans will be healthy and which ones will be high-risk. The financial information data comes from a lending data csv file, and the loan status values is the column of data needed to create the predictions. Using the loan status values from the data set, there are 75,036 healthy loans and 2500 loans that are labeled high-risk. To create this model, the data analyst first split the loan status into training and testing data. Then created a logistic regression model using the original training data. Then the analyst made predictions on the testing data using the created logistic regression model. After this step the accuracy score of the model was evaluated using the balanced_accuracy score, the confusion matrix, and finally a classification report was generated. All of these steps were performed using scikit-learn. The second machine learning process used for this project was a logistic regression model using resampled training data. This second process was carried out using RandomOverSampler in scikit-learn, following the same steps as the first model. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: Logistic Regression
  * Balanced Accuracy: 0.9918 (99%)
  * Precision: 
    - macro avg: 0.92 (92%)
    - weighted avg: 0.99 (99%)
  * Recall: 
    - macro avg: 0.95 (95%)
    - weighted avg: 0.99 (99%)



* Machine Learning Model 2: Logistic Regression with Resampled Training Data
  * Balanced Accuracy: 0.9945 (99%)
  * Precision: 
    - macro avg: 0.99 (99%)
    - weighted avg: 0.99 (99%)
  * Recall:
    - macro avg: 0.99 (99%)
    - weighted avg: 0.99 (99%)

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

Both machine learning models have significantly high accuracy scores and both logistic regression models are worth using. However, it is recommended to use the logistic regression with resampled training data (using the RandomOverSampler) model. This model has a precision of 99% compared to 92% of the first logistic regression model. Since it is more important to predict high risk loans compared to healthy loans, it is necessary to used the resampled (RandomOverSampler) model due to the higher level of accuracy and precision. 

