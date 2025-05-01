# Module 12 Report Template

## Overview of the Analysis

* Purpose:
* * Evaluate the machine learning model’s ability to predict whether a loan is healthy or high-risk.

* Financial Data and My Goal:
* * The data included financial lending information and I needed to predict if the loans tatus.

* Variable – loan status:
* * The prediction focused on the loan_status column.
* * A quick value_counts() of the data showed:
* * * 0: 18,759 (healthy loans)
* * * 1: 625 (high-risk loans)

* Process:
* * Loaded and explored the dataset using pandas.
* * Split the dataset into features (X) and target (y).
* * Used train_test_split to divide the data into training and testing sets with stratification to maintain label balance.
* * Trained the model using the training data.
* * Made predictions on the testing data.
* * Reviewed the model performance using accuracy, precision, recall, and F1 score.

* Methods:
* * The primary model used was LogisticRegression from scikit-learn.
* * Evaluated the model using confusion_matrix and classification_report to assess how well the model predicted both healthy and high-risk loans.

## Results

* Machine Learning Model 1:
* * Accuracy:
* * * The model does a fantastic job predicting both loan labels.

* * Healthy Loans (0 label):
* * * Gave 1.00 in each area — extremely accurate.
* * * Precision shows each loan was predicted correctly.
* * * Recall was perfect on the test set.
* * * F1 score confirms low chance of false positives or negatives.

* * High-Risk Loans (1 label):
* * * Accurate most of the time.
* * * Small chance of getting it wrong.
* * *  Needs fine-tuning to improve accuracy.

## Summary

* I don't recommend that this model is used solely on the purpose that data doesn't tell the full story regarding someone full financial picture. The company that the data is sourced from has lead to questions about the data regarding how the dataset was created, as in, what metrics or processes were used to filter who should be considered? The dataset may not factor in how biases frmo race, gender, income, and etc, influnce. Considering, the company has a direct financial interest in making sure that it can appear to tell who is high and low risk. Overall, it works well. 