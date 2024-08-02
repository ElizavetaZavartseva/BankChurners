# BankChurners
Link for slides presentation: https://www.canva.com/design/DAGMheG0TH8/5ejWERFQDozb-bTKRwDg0A/edit?utm_content=DAGMheG0TH8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton 

Customer Churn Prediction in the Banking Sector
We utilized the "Bank Customer Churn" dataset from Kaggle. Link for dataset: https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers.

Problem
Which customers are at risk of churning (Clients stop using a bank’s services).

Objective
Creating a predictive model and testing data.

Impact 
Understanding the factors that lead to customer churn allows us to enhance customer retention strategies.

Data Preparation:
1. Removed irrelevant columns and handled missing values
2. Converted categorical features into numerical format. Nominal Cathegorical: One Hot Encoding, Ordinal Cathegorical: Label Encoding.
3. Randomly divided the dataset into training and testing sets.
4. Normalized and Scaled the training and testing sets using MinMaxScaler.
5. Feature Selecting: removed some features which had low correlationship with target, and some features that had high corrletions between themselves.

We tested 7 predictive models models with 3 diffrent types of dataset (Original, Normalized, Reduced):

1. KNN
2. Logistic Regression
3. Decision trees
4. Bagging and Pasting
5. Random Patches
6. AdaBoost
7. Gradient Boosting

The most relevant model for this project is Random Patches. This model gave us better recall results which is a general goal for customer churning tasks.

For this model we applied Hyperparameter Tuning.
The highest mean test score is for 'max_depth': 30 and n_estimators': 200. 
The standard deviation of scores is 0.004450 and relatively low across most parameter combinations, indicating stable performance.

Real-World Application and Impact:

Customer Retention: 
Helps identify customers who might leave, so the bank can take steps to keep them.

Resource Allocation:
Focuses efforts on customers who are most likely to leave.

Strategic Decisions:
Provides insights to create better products and marketing plans.







