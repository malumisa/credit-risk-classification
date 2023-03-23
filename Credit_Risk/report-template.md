# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


*  The purpose of the analysis was to develop an algorithm that can learn the the patterns in the dataset and use learning to make predictions. In this applicaiton it was to train and evaluate a model based on loan risk. A dataset of historical lending activity from peer-to-peer  lending services company was made available for building a model that helps identify the creditworthiness of borrowers. First i had to read the lending_data.csv data into a Pandas DataFrame after which i created the labels set (y) from the "loan_status" columnn and also created the features (x) DataFrame from the remaining columns. The data was split into training and testing by using train_test_split.
*  
*  The next step involved creating a Logistic Regressin model with the original data. Here i fitted the logistic regression model using the training data (X_train and y_train). I went on to save the predictions for the testing data labels by using the testing feature dataa (X_test) and the fitted model. 
     
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

It was crucial to evaluate the model's performance by doing the following:
     * calculating the accuracy score of the model
     * generating a confusion matrix
     * printing the classification report
     
* Balanced accuracy score of the model = 95%. This may be attributed to the unbalanced data considering that the number of healthy loans (low-risk) by far exceeds the number og unhealthy loans (high-risk)
* Precision score = 85%
* Recall score = 91%
* 
* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

Balanced accuracy score of the model = 99%. This is higher than for the model fitted with unbalanced data.  We conclude that the oversampled model performs better as it identies mistakes such as labeling non-healthy (high-risk) loans as healthy (low-risk) 

* Precision score = 84%
* Recall score = 99%
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
If you do not recommend any of the models, please justify your reasoning.

* 
