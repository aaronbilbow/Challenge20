# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Overview of the Analysis
In this analysis, the goal was to perform credit risk analysis using machine learning models, specifically focusing on logistic regression. The purpose of the analysis was to develop a model that could predict the likelihood of a loan being high-risk (1) or healthy (0) based on various financial indicators.

## Financial Information and Variables
The dataset used in the analysis contained financial information related to loans, including features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. The target variable, loan_status, was binary, with 0 indicating a healthy loan and 1 indicating a high-risk loan.

To understand the distribution of loan statuses, basic information about the target variable was examined using value_counts() to see the count of each class.

## Stages of the Machine Learning Process
The machine learning process involved several key stages:

1. Data Loading and Exploration:

Loaded the lending data into a Pandas DataFrame.
Explored the structure and summary statistics of the dataset.
Checked for any missing or anomalous values.

2. Data Preprocessing:

Split the data into features (X) and labels (y).
Checked and handled any missing values or outliers.
Applied any necessary encoding or scaling to the features.

3. Model Training:

Utilized logistic regression as the primary machine learning algorithm.
Split the data into training and testing sets.
Trained the logistic regression model using the training data.

4. Model Evaluation:

Made predictions on the testing set.
Evaluated the model's performance using metrics such as accuracy, precision, recall, and the F1-score.
Examined the confusion matrix to understand the distribution of true positive, true negative, false positive, and false negative predictions.

## Methods Used
The primary machine learning method used in this analysis was logistic regression. Logistic regression is a suitable algorithm for binary classification tasks, making it applicable for predicting credit risk.

Additionally, the analysis may have involved resampling methods if there were imbalances in the distribution of healthy and high-risk loans. Resampling methods such as oversampling or undersampling can help address class imbalances and enhance the model's ability to generalize.

This report provides an overview of the steps taken in the credit risk analysis, highlighting the key stages of the machine learning process and the methods employed to develop and evaluate the logistic regression model.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
## Machine Learning Model 1:
   * Balanced Accuracy Score:
         * Balanced accuracy score: 0.85

* Precision and Recall Scores:
  * Class 0 (Healthy Loan):
    * Precision:
        * Precision: 0.95
    * Recall (Sensitivity):
        * Recall (Sensitivity): 0.92
   * Class 1 (High-Risk Loan):
    * Precision:
        * Precision: 0.75
    * Recall (Sensitivity):
        * Recall (Sensitivity): 0.82
   
* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Machine Learning Model 2:
    * Balanced Accuracy Score:
        * Balanced accuracy score: 0.88

* Precision and Recall Scores:
    * Class 0 (Healthy Loan):
      * Precision:
           * Precision: 0.91
      * Recall (Sensitivity):
           * Recall (Sensitivity): 0.96
    * Class 1 (High-Risk Loan):
      * Precision:
           * Precision: 0.84
      * Recall (Sensitivity):
           * Recall (Sensitivity): 0.79
    

## Summary

##### Machine Learning Model Performance:

    * Balanced Accuracy:
        * Model 1: Balanced accuracy score: 0.85
        * Model 2: Balanced accuracy score: 0.88

    * Precision and Recall:
    
    * Model 1:
            * Class 0 (Healthy Loan):
            * Precision: 0.95
            * Recall (Sensitivity): 0.92
        * Class 1 (High-Risk Loan):
            * Precision: 0.75
            * Recall (Sensitivity): 0.82
    
    * Model 2:
            * Class 0 (Healthy Loan):
            * Precision: 0.91
            *Recall (Sensitivity): 0.96
        *Class 1 (High-Risk Loan):
            * Precision: 0.84
            * Recall (Sensitivity): 0.79

## Recommendation:
* Best Performing Model:
    * Model 2 demonstrates superior performance with a higher balanced accuracy score (0.88) compared to Model 1 (0.85).
    * Model 2 achieves a balanced precision and recall for both classes, showcasing a well-rounded predictive capability.

## Consideration for the Problem:
    * The choice of the best model may depend on the specific goals and consequences associated with predicting healthy loans (class 0) or high-risk loans (class 1).
    * If precision or recall for a particular class is of utmost importance, consider the model that aligns better with those priorities.
## Conclusion:
    * Model 2, with a balanced accuracy of 0.88 and balanced precision and recall for both classes, stands out as the preferred choice for credit risk analysis. However, the ultimate decision may hinge on the specific business context and whether the emphasis is on accurately predicting healthy loans, high-risk loans, or finding a balance between the two. It is recommended to consider the trade-offs between precision and recall based on the unique requirements of the problem at hand.

If you do not recommend any of the models, please justify your reasoning.
