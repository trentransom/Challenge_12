# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to created a model that would accurately predict whether a potential loan is healthy or high-risk. 
Our data included information about the size of the loan, interest rate, borrower income, borrower debt-to-income ratio, number of accounts, derogatory marks, and total debt. We are predicting the status of the loan based on these features. 
In our data we had 75,036 instances of a healthy loan and 2500 instances of a high-risk loan. 
Before we began building the model we split our data into training data and testing data with a 75/25 split. 
We chose to use logistic regression as the model for machine learning. We then fit our model to the training data and made predictions based on the testing data. We then evaluated those predictions against the known values from our original dataset. 
We then repeated this process but before fitting the model we oversampled the high-risk loans so they would be equally represented in the dataset. 

## Results

* Machine Learning Model 1:
  * Accuracy: 94.5%
  * Precision: 
    * Healthy: 100% 
    * High-Risk: 88%
  * Recall:
    * Healthy: 100%
    * High-Risk: 90%


* Machine Learning Model 2:
  * Accuracy: 99.5%
  * Precision:
    * Healthy: 100%
    * High-Risk: 87%
  * Recall:
    * Healthy: 99%
    * High-Risk: 100%

## Summary

Machine Learning Model 2 seems to perform the best. It has a higher overall accuracy and recall for the high-risk loan class improved dramatically. All other metrics remained about the same. 
Whether we care more about predicting the larger or smaller class or precision over recall depends on the problem we are trying to solve. In this case, we want the model to be very good at predicting high-risk loans as those will be harmful to our business. We can feel comfortable using this model since the recall for high-risk loans is so high. That means we know that there are very few high-risk loans that the model will not accurately predict. We know that using this model, nearly all the loans we approve will be healthy loans. 
