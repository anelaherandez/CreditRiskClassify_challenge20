# CreditRiskClassify_challenge20
In this Challenge, use various techniques to train and evaluate a model based on loan risk. Using a dataset of historical lending activity from a peer-to-peer lending services company the data analyst will build a model that can identify the creditworthiness of borrowers.

The instructions for this Challenge are divided into the following subsections:
Split the Data into Training and Testing Sets
Create a Logistic Regression Model with the Original Data
Write a Credit Risk Analysis Report

## Split the Data into Training and Testing Sets
Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
Split the data into training and testing datasets by using train_test_split.

## Create a Logistic Regression Model with the Original Data
Fit a logistic regression model by using the training data (X_train and y_train).
Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
Evaluate the model’s performance by doing the following:
Generate a confusion matrix.
Print the classification report.

## Create a Logistic Regression Model with Resampled Training Data (using RandomOverSampler in Scikit-Learn)
Fit a logistic regression model by using resampled training data using the RandomOverSampler metric in Scikit-learn(X_ros_model and y_ros_model).
Save the predictions for the testing data labels by using the testing feature data (X_ros_model) and the fitted model.
Evaluate the model’s performance by doing the following:
Generate a confusion matrix.
Print the classification report.

## Analysis Report
Both machine learning models have significantly high accuracy scores and both logistic regression models are worth using. However, it is recommended to use the logistic regression with resampled training data (using the RandomOverSampler) model. This model has a precision of 99% compared to 92% of the first logistic regression model. Since it is more important to predict high risk loans compared to healthy loans, it is necessary to used the resampled (RandomOverSampler) model due to the higher level of accuracy and precision.