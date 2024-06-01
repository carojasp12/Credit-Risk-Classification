# Credit-Risk-Classification
![image](https://github.com/carojasp12/Credit-Risk-Classification/assets/152667250/0f0dbc32-1635-4457-bd18-f0dcaa3ae539)

## Overview of the Analysis
In this project, various techniques were employed to train and evaluate a model designed to assess loan risk. Utilizing a dataset of historical lending activity from a peer-to-peer lending services company, the goal was to construct a model capable of finding the creditworthiness of borrowers. The process involved splitting the data into training and testing sets and applying a logistic regression model with the original data to predict loan status. The peer-to-peer lending services dataset includes the following variables:
•	loan_size
•	interest_rate
•	borrower_income
•	debt_to_income
•	num_of_accounts
•	derogatory_marks
•	total_debt
•	loan_status

### Split the Data into Training and Testing Sets
To begin the analysis, we first split the data into training and testing sets as follows:

1.	We start by reading the lending_data.csv file into a Pandas DataFrame.
2.	We create the labels set (y) from the "loan_status" column. Then, we create the features (X) DataFrame by selecting the remaining columns from the dataset.
3.	We split the data into training and testing datasets using the train_test_split function from the sklearn.model_selection module.
   
### Create a Logistic Regression Model with the Original Data
We use logistic regression due to its effectiveness in binary classification tasks to predict loan risk. The following steps outline the process:

1.	We fit the logistic regression model with the training data (X_train and y_train). This process trains the model to learn the relationship between the features and the loan status.
2.	Using the fitted model, we generate predictions for the testing data labels. This involves using the testing feature data (X_test) to predict the risk level of the loans.
3.	To evaluate the performance of the model, we generate a confusion matrix and print a classification report to assess the model's accuracy, precision, recall, and F1-score.


