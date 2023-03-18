# credit-risk-classification

## Overview of the Analysis
In this challenge I used historical peer-to-peer lending data to predict creditworthiness. The data set included several features including the borrower's income, interest rate, debt to income ration, etc. I selected loan status as the dependent variable that corresponded with borrower's creditworthiness. A '1' variable indicates that a borrower has an elevated potential for defualt, '0' indicates the opposite.  I built two models using a logistic regression (using orignal and resampled training data) module to train a portion of the data set.  I then fed the remaining data into the model to predict the loan status. Finally, I compared the predicted values to those in the original data set and analyzed the result. 

## Results

* Machine Learning Model 1 (original data):
    * Accuracy:  This model scored approx. 0.95 for accuracy which indicates that the model is very good at predicting creditworthiness
    * Precision: The model was always right when it classified a loan as a healthy, but only correct 85% of the time when it classified a loan as a high risk for default. 
    * Recall: The recall is .99 for healthy loans and .91 or high risk loans. So, the model is pretty good at putting healthy and unhealthy loans in their correct buckets.
  


* Machine Learning Model 2 (resampled data):
    * Accuracy:  This model scored approx. 0.99 for accuracy which indicates that the model is verygood at predicting creditworthiness
    * Precision: The model was always right when it classified a loan as a healthy, but only correct 84% of the time when it classified a loan as high risk for default.
    * Recall: The recall is .99 for both high risk loans and healthy loans. So overall, the model is very good at classifying the loans correctly. 


## Summary
Both models preform well, with the second model performing slightly better. Since high risk loans present an issue for lenders, our goal is to have a model that is better at predicting high risk loans. In this case I would reccomend the second model.  Although we do sacrifice a tiny bit of precision,  both the accuracy and recall are higher than that of the first model.  

