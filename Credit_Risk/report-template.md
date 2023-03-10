# Module 12 Report produced by Vincent Passanisi

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is to build a prediction model that will be able to analyze credit worthiness of borrowers for the bank and flag potential loan defaults. The dataset provided by the bank contains 77,536 entries with seven key indicators. These are listed as follows:

* Size of the loan
* Interest rate on the loan
* Borrower's income 
* Debt_to_Income ratio
* The number of of accounts that the borrower uses regularly
* derogatory marks on the borrower's credit report
* The borrower's total debt

A final column called *loan status* is provided that indicates whether the borrower defaulted on the loan. A 1 indicates that the borrower defaulted, a '0' indicates a healthy loan.

In the dataset there are 2500 loans out of the 77,536 that are in default. This was determined by getting the value counts of the *loan status* column. These loan defaults make up 3.22% of the bank's loans for the information provided in the dataset. Total loans made amounted to $760,284,100. Of this total, the 2,500 loans in default amounted to $46,269,501 or 6.09% of the assets on loan. Obviously, this amount is disproportionate to the number of loans in default, and the bank owes a fiduciary duty to it's stockholders to limit this amount to any degree possible.

The data was first split to remove the *loan status* column and save it as a separate data frame to be used as labels. The data features were then split into training data and testing data. This was done using a default 75/25 split. The training data was then fit to a Logistic Regregression model. Scoring the model resulted in a training score of *Training Data Score* of **0.99212** and a *Testing Data Score* of **0.99184**. The model was then used to predict the test data and indicators were generated for balanced accuracy score, confusion matrix, and a classification report.

The testing data was then subjected to random oversampling of the loan default status. The purpose of this is to over-represent the default loans in the dataset in order to better test the models predictive power. The resulting random data was composed of equal data points of 75,036 for both healthy loans(**0**) and default loans (**1**). A new model was fit using Logistic Regression for the resampled data, and then this data was used to predict the original test data. Once again, a balanced accuracy score, confusion matrix, and classification report were generated from the results.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
