# Credit Risk Classification Report

## Analysis Overview
The purpose of this analysis was to build a two different models that tests historical lending data to assess the credit of potential borrowers. Based on the output of these models, one can identify which model is more accurate than the other (if any). The financial information, in a broad sense, covers different aspects of lending data. More specifically, the size of each loan, interest rate, the borrower's income, the borrower's debt to income ratio, etc. Based on this information, each model is trying to predict which borrowers in this dataset carry a high-risk in taking a loan vs. which borrowers carry a healthy risk in taking a loan.
In order to build each model, the raw data needed to split into training and testing sets. The "loan_status" is what the model is trying to predict, producing a binary outcome of 0 or 1; healthy loan and high-risk loans respectively. The remaining data is what the model is using to determine which category a particular borrower falls in. Once the data has been split into training and testing sets, the models are built. This is done with the logistic regression model, where the training data is fit in. Using this model, the testing data is inputted and predicted and stored in an array. From there the confusion matrix, the balanced accuracy score and the classification report can be generated. The second model follows a similar procedure, however the data is first resampled before being fit into the linear regression model.

## Results
* Machine Learning Model 1: Logisitic Regression Model Using Original Data
  * This model produced a balanced accuracy score of 95%.
  * Below is a sample of the confusion matrix results: 
  
    ![Confusion Matrix](module_12_challenge/confusion_matrix_1.png)

  * Below is a sample of the classification report results: 
    
    ![Classification Report](classification_report.png)

* Machine Learning Model 2: Logisitic Regression Model Using Resampled Data
  * This model also produced a balanced accuracy score of 95%.
  * Below is a sample of the confusion matrix results: 
  
    ![Confusion Matrix](confusion_matrix_1.png)

  * Below is a sample of the classification report results: 
    
    ![Classification Report](classification_report.png)

## Summary
From the given results, both models produce the exact same scores in terms of precision, recall and accuracy. The precision score for both models is perfect for the healthy loan, but is relatively poorer for the high-risk loans. The recall score follows the same pattern as the precision score in terms of which outcome scores better, but overall, it produces better results than the precision score. Hence, if there is more of an emphasis on the importance of the recall score, then either model would be better suited for that, since both models produced the same results.
