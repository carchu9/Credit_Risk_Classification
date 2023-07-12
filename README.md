# Credit_Risk_Classification

## Purpose
The purpose of the analysis is to build a model that can determine and identify if an applicant would be considered a "healthy loan" applicant or a "high risk" applicant. The factors that would determine this would be interest rate, loan size, number of accounts, borrower income, debt to income ratio, derogatory marks against the borrower and total debt. 

## Proccess
The data is split into two sets, training and tests. The training set was then used to create an initial Logistic Regression Model using the LogisticRegression, a dependency from scikit-learn. 

Resampling the training data is needed to ensure there are no imbalances. The data was resampled by using the RandomOverSampler module from imbalanced-learn. The process to create the initial Logicstic Regression Model was then applied to the second resampled set to create the second Logistic Regression Model. 

Using the Logistic Regression Models, two sepearte confusion matrixes were created to test the accuracy and precision of the data for both sets.

## Results

Logistic Regression Model 1:
![image](https://github.com/carchu9/Credit_Risk_Classification/assets/122560104/c198bcba-558e-4002-9c21-26eb613a8a2e)
* Balanced  Score: ![image](https://github.com/carchu9/Credit_Risk_Classification/assets/122560104/48f43e47-e610-4dea-8436-e41217519736)

* Balanced Accuracy: 99%
* Precision for Healthy Loans: 100%
* Precision for High Risk Loans: 87%
* Recall for Healthy Loans:  100%
* Recall for High Risk Loans: 89%

Logistic Regression Model 2:
![image](https://github.com/carchu9/Credit_Risk_Classification/assets/122560104/aedb8481-451a-4691-8aab-cf9312f3d56f)
* Balanced Score: ![image](https://github.com/carchu9/Credit_Risk_Classification/assets/122560104/ffceb192-a52d-43cc-a30d-93cdaa36c637)

* Balanced Accuracy: 100%
* Precision for Healthy Loans: 100%
* Precision for High Risk Loans: 87%
* Recall for Healthy Loans: 100%
* Recall for High Risk Loans: 100%

## Summary

The first logistic regression model showed 100% precision, and recall when predicting the healthy loan applicants and an accuracy of 99%. However, when determining the high risks loan applicants performs with less precision, and recall. The first model demonstrates it's inability to determine high-risk loan applicants. 

The second logistic regression model shows a better accuracy, precision and recall score when identifying high risks loan applicants. 

The second model is recommended as it will be able to identify high risk loan applicants with better accuracy. This is important as most banks and lenders are less likely to loan to borrowers who are high risk. 
