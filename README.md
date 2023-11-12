# credit-risk-classification

# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to predict credit risk for loans using machine learning models. The financial data provided details on loans like loan size, interest rate, income, debt level, etc. The goal was to predict if a loan was high risk (1) or healthy (0).

I went through the machine learning process of splitting data, fitting and evaluating models, and tuning models. I used LogisticRegression on the original imbalanced data and then resampled with RandomOverSampler to handle class imbalance.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.94
  * Precision: 0.99 for 0 class, 0.87 for 1 class
  * Recall: 1.00 for 0 class, 0.89 for 1 class

* Machine Learning Model 2:
  * Balanced Accuracy Score: 0.99
  * Precision: 0.99 for both 0 and 1 classes
  * Recall: 0.99 for both 0 and 1 classes.

## Summary

The oversampled LogisticRegression model performed best, with significantly improved scores over the original model.

On the imbalanced data, the model strongly favored the majority 0 class, as evidenced by the high 1.0 precision but only 0.89 recall on the 1 class.

Oversampling created equal samples of each class, which enabled the model to improve precision and recall to 0.99 for both classes.

I recommend the oversampled LogisticRegression model because it does an excellent job predicting both the healthy (0) and high-risk (1) loans with a high level of accuracy. The oversampling corrected the initial class imbalance problem and resulted in a model that performs very well for this credit risk classification task.


## Instructions
The instructions for this Challenge are divided into the following subsections:
 - Split the Data into Training and Testing Sets
 - Create a Logistic Regression Model with the Original Data
 - Write a Credit Risk Analysis Report

## Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:
 1. Read the `lending_data.csv` data from the Resources folder into a Pandas DataFrame.
 2. Create the labels set (`y`) from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.
    >[!NOTE]
    >A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

 3. Split the data into training and testing datasets by using `train_test_split`.

## Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:
 1. Fit a logistic regression model by using the training data (`X_train` and `y_train`).
 2. Save the predictions for the testing data labels by using the testing feature data (`X_test`) and the fitted model.
 3. Evaluate the model’s performance by doing the following:
    - Generate a confusion matrix.
    - Print the classification report.
 4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

## Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the `README.md` file included in your GitHub repository.

Structure your report by using the report template that `Starter_Code.zip` includes, ensuring that it contains the following:

  1. **An overview of the analysis**: Explain the purpose of this analysis.
  2. **The results**: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
  3. **A summary**: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

# Analysis Report
Here goes the analysis.
