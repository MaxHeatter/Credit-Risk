# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Purpose
This module was designed to create a Logistic Regression Model that can accurately predict healthy from high-risk loan statuses.

## Data
This analysis used the lending_data.csv file which had information on the individual's income, total debt, debt-to-income ratio, number of other accounts, derogatory credit marks principal, and interest rate. 

The data also featured a column for loan status differentiating the difference between a healthy loan 0, and a high-risk loan 1.

## Process
To start on the analysis the creation of a Logistic Regression model with the original data set was needed. After fitting and redicting with this model it is able to yield its accuracy, confusion matrix scores, as well as its classification report for analysis on how well the model performed. The second model used over sampled data instead after the use of RandomOverSampler. This model was fit and predicted similar to the first model, but with different data given yielded osme slightly different results.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

### Machine Learning Model 1:

- Balanced Accuracy Score: 0.9520479254722232 (95.2%)
    - Healthy Loans:
        Precision: 1.00 (100%)
        Recall: 0.99 (99%)
    - High-risk Loans:
        Precision: 0.85 (85%)
        Recall: 0.91 (91%)

### Machine Learning Model 2:

- Balanced Accuracy Score: 0.9936781215845847 (99.7%)
    - Healthy Loans:
        Precision: 1.00 (100%)
        Recall: 0.99 (99%)
    - High-risk Loans:
        Precision: 0.84 (84%)
        Recall: 0.99 (99%)
## Summary
The second model did almost everything better than the first model, barring the precision score dropping 1% in the high-risk category, however I do believe the it to be better with higher balanced accuracy 99% > 95% and a higher recall score 99% > 91%. With this data set the high-risk individuals are more important to be accurate on and even though there is a 1% decrease in precision, the recall score increases enough to cover this loss and use the model evn though there is room for improvement.
