# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The *purpose* of this analysis is to evaluate the machine learning models to predict whether a loan is classifed as **healthy loan (0)** or **high-risk loan (1)** and if the model is well suited to be deployed for automating loan approvsal processes to *minimise the financial risk*

* Explain what financial information the data was on, and what you needed to predict.

The data contained the following information:

	loan_size
    interest_rate	
    borrower_income	
    debt_to_income	
    num_of_accounts	
    derogatory_marks	
    total_debt

The target variable had two values which are 0 for healthy loans and 1 for high-risk loans.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

* Describe the stages of the machine learning process you went through as part of this analysis.

While preparing the analysis I followed the following steps:
1. **Data Preparation:** Split the data into features (x) and labels (y) and then scaling the data using standard scaler.
2. **Model Training:** Trained the model.
3. **Model Evaluation:** Assessed the model performance for `accuracy`, `recall` and `F1-score.`

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

The mothods which I used to classify the loan status are `logistic regression` and `standard scalar` is used for data scaling.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

    * **Accuracy: 99%**
     The model correctly classified 99% of loans in the testing dataset.

    *  **Precision:**

     Healthy loans (0): 100% (perfect precision; no false positives).

     High-risk loans (1): 84% (some false positives).

    * **Recall:**

     Healthy loans (0): 99% (almost all healthy loans correctly identified).

     High-risk loans (1): 99% (almost all high-risk loans correctly identified).

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?

The **logistic regression** model performed well based on high accuracy and recall scores for both *healthy and high-risk loans*.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

**Yes**, the performance depends on identifying the high-risk loans `1` or healthy loans `0`. Identifying `high-risk loans 1's` is more important because it would lead to financial losses if these loans are oversighted.
