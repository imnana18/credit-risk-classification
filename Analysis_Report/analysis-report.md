# Module 12 Analysis Report

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of the analysis is to construct and evaluate a predictive model for identifying the creditworthiness of borrowers using historical lending data from a peer-to-peer lending services company. The dataset provided, lending_data.csv, contains information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. Based on these features, we are predicting the loan status of borrowers. 

We split the dataset into testing and training variables to fit four different machine learning models to predict whether a loan is high-risk (label 1) or healthy (label 0) based on the provided features. The models tested for this dataset include Linear Regression, SVM, Random Forest, and KNN models in listed order. The classification reports provides an evaluation of the model's performance in terms of precision, recall, and F1-score for both the high-risk and healthy loan categories.

On a larger scale, by understanding patterns and relationships within the data and leveraging machine learning techniques, the objective is to identify a model that most accurately assesses the risk associated with loans, enabling the lending company to make informed decisions about lending practices and manage potential risks effectively.

## Results

* Logistic Regression:
    - For label 0 (healthy loan):
        ***Precision:*** The precision for healthy loans is 1.00, which indicates that when the model predicts a loan as healthy (label 0), it is correct 100% of the time.
        
        ***Recall:*** For label 0, the recall is 0.99, indicating that the model correctly identifies 99% of the healthy loans.

        ***F1-score:*** The F1-score is the harmonic mean of precision and recall. For label 0, the F1-score is 1.00, indicating high accuracy in predicting healthy loans.

    - For label 1 (high-risk loan):
        ***Precision:*** The precision is 0.84, indicating that when the model predicts a loan as high-risk (label 1), it is correct about 84% of the time.

        ***Recall:*** The recall for label 1 is 0.94, indicating that the model correctly identifies about 94% of the high-risk loans.

        ***F1-score:*** The F1-score for label 1 is 0.89, which suggests a good balance between precision and recall for predicting high-risk loans.

    Overall, the logistic regression model performs well in predicting both healthy loans and high-risk loans. It achieves near-perfect precision and recall for healthy loans (0) and reasonably high precision and recall for high-risk loans (1). 

* SVM Model:
    - For label 0 (healthy loan):
        ***Precision:*** The precision for healthy loans is 1.00, which indicates that when the model predicts a loan as healthy (label 0), it is correct 100% of the time.
        
        ***Recall:*** The recall is 0.99, indicating that the model correctly identifies 99% of the healthy loans.

        ***F1-score:*** The F1-score is 1.00, indicating high accuracy in predicting healthy loans.

    - For label 1 (high-risk loan):
        ***Precision:*** The precision is 0.84, indicating that when the model predicts a loan as high-risk (label 1), it is correct about 84% of the time.

        ***Recall:*** The recall for label 1 is 0.98, indicating that the model correctly identifies about 98% of the high-risk loans.

        ***F1-score:*** The F1-score for label 1 is 0.91, which suggests a good balance between precision and recall for predicting high-risk loans.

    Overall, the SVM model performs well in predicting both healthy loans and high-risk loans. It achieves near-perfect precision and recall for healthy loans (0) and reasonably high precision and recall for high-risk loans (1). 

* Random Forest Model:
    - For label 0 (healthy loan):
        ***Precision:*** Precision is 1.00, which indicates that when the model predicts a loan as healthy (label 0), it is correct 100% of the time.
        
        ***Recall:*** Recall is 0.99, indicating that the model correctly identifies 99% of the healthy loans.

        ***F1-score:*** The F1-score is 1.00, indicating high accuracy in predicting healthy loans.

    - For label 1 (high-risk loan):
        ***Precision:*** Precision is 0.85, indicating the model is correct about 85% of the time when predicting a loan of high-risk.

        ***Recall:*** The recall for label 1 is 0.90, indicating that the model correctly identifies about 90% of the high-risk loans.

        ***F1-score:*** The F1-score for label 1 is 0.87, which suggests a decent balance between precision and recall for predicting high-risk loans.

    Overall, the Random Forest model performs excellent in predicting healthy loans, but is only decent when looking at high-risk loans. It achieves near-perfect precision and recall for healthy loans (0) and reasonable precision with slightly lower recall for high-risk loans (1). 

* K Nearest Neighbor Model:
    - For label 0 (healthy loan):
        ***Precision:*** Precision is 0.99, which indicates that when the model predicts a loan as healthy (label 0), it is correct 99% of the time.
        
        ***Recall:*** Recall is 1.00, indicating that the model correctly identifies 100% of the healthy loans.

        ***F1-score:*** The F1-score is 0.99, indicating high accuracy in predicting healthy loans.

    - For label 1 (high-risk loan):
        ***Precision:*** Precision is 0.85, indicating the model is correct about 85% of the time when predicting a loan of high-risk.

        ***Recall:*** The recall for label 1 is 0.74, indicating that the model correctly identifies only about 74% of the high-risk loans.

        ***F1-score:*** The F1-score for label 1 is 0.79, which suggests only a moderately decent balance between precision and recall for predicting high-risk loans.

    Overall, the KNN model performs excellent when predicting healthy loans, but is somewhat lackluster when looking at high-risk loans compared to our other models. It achieves near-perfect precision and recall for healthy loans (0) and reasonable precision but much lower recall for high-risk loans (1). 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

While the four models each are relatively good at predicting loan status of the data, especially for healthy loans, SVM model seems to be the best choice for this dataset. 

Considering that the main focus is predicting loan status, we want high precision and recall for both types of loans (healthy and risky). SVM model has high precision for both healthy and high-risk classes and most noteably, the highest recall score for risky loans among all the models. While all four models prove excellent at predicting loan status for healthy loans, only the SVM model shows an astounding 98% accuracy when correctly identifying high-risk loans. 

This means that the SVM model shows relatively balanced performance in identifying both types of loans. Additionally, it has the highest F1-score for high-risk loans among the models considered, suggesting better overall performance in capturing true positives while minimizing false positives and false negatives. 

