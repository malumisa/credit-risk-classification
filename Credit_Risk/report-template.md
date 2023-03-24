# Module 12 Report Template

## Overview of the Analysis

*  The purpose of the analysis was to develop an algorithm that can learn the the patterns in the dataset and use learning to make predictions. In this applicaiton it was to train and evaluate a model based on loan risk. A dataset of historical lending activity from peer-to-peer  lending services company was made available for building a model that helps identify the creditworthiness of borrowers. First i had to read the lending_data.csv data into a Pandas DataFrame after which i created the labels set (y) from the "loan_status" columnn and also created the features (x) DataFrame from the remaining columns. The data was split into training and testing by using train_test_split.
*  
*  The next step involved creating a Logistic Regressin model with the original data. Here i fitted the logistic regression model using the training data (X_train and y_train). I went on to save the predictions for the testing data labels by using the testing feature dataa (X_test) and the fitted model. 
     
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
     
 <img width="561" alt="image" src="https://user-images.githubusercontent.com/111699427/227403793-75428202-185c-401f-88fc-7ad90bc25f99.png">
     
 <img width="807" alt="image" src="https://user-images.githubusercontent.com/111699427/227403864-451246bb-72be-47ba-851c-d0469a99b91f.png">

* Balanced accuracy score of the model = 95%. This may be attributed to the unbalanced data considering that the number of healthy loans (low-risk) by far exceeds the number og unhealthy loans (high-risk)
* Precision score = 85%
* Recall score = 91%

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

<img width="601" alt="image" src="https://user-images.githubusercontent.com/111699427/227403921-48961258-244f-4660-a6d3-764dffdad258.png">

Balanced accuracy score of the model = 99%. This is higher than for the model fitted with unbalanced data.  We conclude that the oversampled model performs better as it identifies mistakes such as labeling non-healthy (high-risk) loans as healthy (low-risk) 

* Precision score = 84%
* Recall score = 99%

## Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* The second model perfoms best as it has a higher balanced accuracy score  at 99% 
* For this analysis it is more important to predict the '0''s (healthy loan) to reduce high default rate from 
* I am recommending the second model as it does a better job in identifying mistakes of the first model, which may have labelled high-risk loans as low risk. This is based on the recall score increasing from the imbalanced model to the oversampled model
