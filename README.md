# credit-risk-classification

## Overview of the Analysis
The purpose of this analysis is to find the best model to successfully indentify the creditworthly of borrowrres from a dataset of historical lending activity from a peer-to-peer lending services company. The dataset provides various information about the borrowers such as the loan size, interest rate, their income, total debts, loan status, and so on... with the main task is to find a model successfully identify which account is healthly loan and which account is high-risk loan. 

Using logistic regression model could be the most efficiency and low cost model for predicting binary outcome from a dataset. With the current dataset, a logistic regression model will train the data and validate the data before making the prediction to increase the accuracy of the model.

## Results

![Alt text](<testing report.png>)

The classification report for the logistic regression model shows excellent performance, especially for predicting the '0' label, which represents healthy loans.

Label '0' (Healthy Loan):
Precision: 1.00, indicating that it is perfectly correct predicts a loan is healthy.
Recall: 1.00, meaning that the model successfully identifies 100% of all healthy loans.
F1-Score: 1.00, showing a perfect balance between precision and recall for healthy loans.
Support: 18,759, representing the number of actual instances of healthy loans in the test dataset.

Label '1' (High-Risk Loan):
Precision: 0.87, suggesting that when the model predicts a loan is high-risk, it is correct 87% of the time.
Recall: 0.95, indicating that the model identifies 95% of all high-risk loans.
F1-Score: 0.91, showing a strong balance between precision and recall for high-risk loans.
Support: 625, representing the number of actual instances of high-risk loans in the test dataset.


## Summary

Overall, the model performs very well for both labels. With perfect precision and recall scores, the model identify perfectly the healthy loan. The model is still identify very good on the high-risk loan account with 87% correct of the time, making it reliable for identifying the majority if high-risk loan. The f1-score for both labels are high, meaning that the model is strong in predictiong loan health status.

Although this model predict better at the healthy loan compared to the high-risk loan, the model excels at predicting for boths. The recall value for `1` is 0.95 which is very high in catching the most positive case. Therefore, this model is suitable to predicting the healthy loan and high-risk loan based on this dataset.
