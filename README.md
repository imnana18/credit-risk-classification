# Credit Risk Classification Challenge

## Background

The objective of this project was to develop a model for assessing loan risk using various machine learning techniques. The dataset provided contained historical lending activity from a peer-to-peer lending services company with the goal to build a model that accurately identified the creditworthiness of borrowers, distinguishing between healthy loans (0) and high-risk loans (1).

## Assignment Map

📁 Analysis_Report
 - `analysis-report.md`: Report analysis for the project.

 


## Files

The necessary files were downloaded from the following link: [Module 20 Challenge files](link-to-files).

## Instructions

The project instructions were divided into the following subsections:

### Splitting the Data into Training and Testing Sets

- The `lending_data.csv` data was read into a Pandas DataFrame.
- The labels set (y) was created from the “loan_status” column, and the features (X) DataFrame was created from the remaining columns.
- The data was split into training and testing datasets using `train_test_split`.

### Creating a Logistic Regression Model with the Original Data

- A logistic regression model was fitted using the training data (`X_train` and `y_train`).
- Predictions for the testing data labels were saved using the testing feature data (`X_test`) and the fitted model.
- The model’s performance was evaluated by:
  - Generating a confusion matrix.
  - Printing the classification report.
  - Answering a critical question regarding the model's prediction accuracy for both healthy and high-risk loans.

### Writing a Credit Risk Analysis Report

- A brief report was prepared summarizing and analyzing the performance of the machine learning models used in this project.
- The provided report template was utilized to structure the analysis, covering:
  - An overview of the anal
