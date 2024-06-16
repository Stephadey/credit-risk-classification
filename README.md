# Module 12 Credit Risk Analysis

## Overview of the Analysis

In this analysis, we developed a logistic regression model to predict the creditworthiness of borrowers using historical lending data from a peer-to-peer lending services company. The primary goal was to accurately classify loans as either healthy (0) or high-risk (1).

The dataset contains the following financial information:

-   **Loan size**
-   **Interest rate**
-   **Borrower income**
-   **Debt-to-income ratio**
-   **Number of accounts**
-   **Derogatory marks**
-   **Total debt**

The target variable is  `loan_status`, which indicates whether a loan is healthy (0) or high-risk (1).

### Stages of the Machine Learning Process:

1.  **Data Loading and Review**: Loaded the lending data into a Pandas DataFrame and reviewed its structure.
2.  **Data Splitting**: Split the data into features (X) and labels (y), and then divided it into training and testing datasets.
3.  **Model Training**: Used the  `LogisticRegression`  algorithm to train the model on the training data.
4.  **Model Prediction**: Made predictions on the testing dataset.
5.  **Model Evaluation**: Evaluated the model's performance using confusion matrix and classification report metrics.

## Results

-   **Machine Learning Model 1: Logistic Regression**
    -   **Accuracy Score**: 0.99
    -   **Precision Score**:
        -   For healthy loans (0): 1.00
        -   For high-risk loans (1): 0.86
    -   **Recall Score**:
        -   For healthy loans (0): 0.99
        -   For high-risk loans (1): 0.94

## Summary

The logistic regression model demonstrates excellent performance in predicting loan statuses. The overall accuracy is very high at 99%, indicating that the model correctly classifies the vast majority of loans.

### Performance Analysis:

-   **Healthy Loans (0)**:
    -   **Precision**: 1.00 (perfect identification of healthy loans)
    -   **Recall**: 0.99 (almost all actual healthy loans are identified)
-   **High-Risk Loans (1)**:
    -   **Precision**: 0.86 (most high-risk loans are correctly identified, but some healthy loans are misclassified as high-risk)
    -   **Recall**: 0.94 (most high-risk loans are correctly identified)

### Recommendation:

The logistic regression model is highly effective and can be recommended for use by the company to predict loan risk. It performs exceptionally well in identifying healthy loans with perfect precision and high recall. The model is also strong in identifying high-risk loans, though there is slight room for improvement in precision.

For this particular problem, accurately predicting both healthy loans and high-risk loans is crucial. Given the high accuracy, precision, and recall scores, this logistic regression model is suitable for deployment in predicting loan statuses and managing credit risk effectively.
