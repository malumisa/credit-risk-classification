# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


*  The purpose of the analysis was to train and evaluate a model based on loan risk. A dataset of historical lending activity from peer-to-peer  lending services company was made available for building a model that helps identify the creditworthiness of borrowers. First i had to read the lending_data.csv data into a Paandas DataFrame after which i created the labels set (y) from the "loan_status" columnn and also created the features (x) DataFrame from the remaining columns. The data was split into training and testing by using train_test_split
*  The next step involved creating a Logistic Regressin model with the original data. Here fit the logistic regression model using the training data (X_train and y_train). I went on to save the predictions for the testing data labels by using the testingfeature dataa (X_test) and the fitted model. It was crucial to evaljuate the model's performance by doing the following:
     * calculating the accuracy score of the model
     * generating a confusion matrix
     * printing the classification report
     
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
