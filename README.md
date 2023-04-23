# Credit Risk Classification Challenge

---

## Summary

This assignment involves utilising Supervised Machine Learning methods to classify and perform predictions and analysis on Credit Risk data.

---

## Required Dependancies

N/A - All required libraries are referenced in the .ipynb file to ensure the code runs as expected. These include;

  - the Pandas library 
  - the Sklearn library 

---

## Credit Risk Analysis Report

### Overview of the Analysis

The aim of this analysis was to develop a model to identify the creditworthiness of borrowers using historical lending data from a peer-to-peer lending service. The initial dataset contained more healthy loan samples than high-risk loan samples. 

To address this imbalance, we used the Random Oversampler method to resample the data and balance out the count of each category type. We trained and tested two logistic regression models: one on the initial data, and one on the resampled data.

### Results

* Model 1: Trained on initial data
    * Accuracy: 0.99
    * Precision: 1.0 for healthy loans, 0.87 for high-risk loans
    * Recall: 1.0 for healthy loans, 0.89 for high-risk loans

* Model 2: Trained on resampled data
    * Accuracy: 0.94
    * Precision: 0.90 for healthy loans, 0.99 for high-risk loans
    * Recall: 0.99 for healthy loans, 0.89 for high-risk loans

### Summary

Based on the results, Model 1 was able to predict healthy loans with great accuracy but did not perform as well for high-risk loans. On the other hand, Model 2 provided an increase in performance for high-risk loans without sacrificing too much for healthy loans. 

Given the context of the data and the need to identify high-risk loans, I would recommend using Model 2 to predict if a customer is a risk or not. 

However, it's important to note that the model's performance may vary depending on the specific dataset used, and further testing and validation may be necessary before deploying the model in a real-world application.

---

## Working Notes

This challenge was good continuation into machine learning, and felt far more comfortable than unsupervised learning. The idea of training the model before applying the test data to it is a concept i'm interested in persuing further into it's praxctical applications. 

---

## Criteria

The marking criteria reads as follows;
### Split the Data into Training and Testing Sets (30 points)
- [x] Read the lending_data.csv data from the Resources folder into a Pandas DataFrame. (5 points)
- [x] Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns. (10 points)
- [x] Split the data into training and testing datasets by using train_test_split. (15 points)

### Create a Logistic Regression Model (30 points)
- [x] Fit a logistic regression model by using the training data (X_train and y_train). (10 points)
- [x] Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. (5 points)
- [x] Generate a confusion matrix. (5 points)
- [x] Generate a classification report. (5 points)
- [x] Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels? (5 points)

### Write a Credit Risk Analysis Report (20 points)
- [x] Provide an overview that explains the purpose of this analysis. (5 points)
- [x] Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)
- [x] Summarise the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

### Coding Conventions and Formatting (10 points)
- [x] Place imports at the top of the file, just after any module comments and docstrings, and before module globals and constants. (3 points)
- [x] Name functions and variables with lowercase characters, with words separated by underscores. (2 points)
- [x] Follow DRY (Don't Repeat Yourself) principles, creating maintainable and reusable code. (3 points)
- [x] Use concise logic and creative engineering where possible. (2 points)

### Code Comments (10 points)
- [x] Be well commented with concise, relevant notes that other developers can understand. (10 points)

---

## Other Comments

A solid week - looking forward to getting stuck into Nerual Networks and hitting the home stretch!
