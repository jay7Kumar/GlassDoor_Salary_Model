# GlassDoor_Salary_Model

#Data Science Salary Estimator Project Overview
-Created a tool that estimates Data Science salaries to help data scientists understand the current pay scale in the job market.
-Used dataset from glassdoor 
-Engineered features from the text of job description to quantify the vlue companies put on Python, SQl, excel, AWS.
-Optimised Linear , Lasso, RandomForest Regressors using GridSearchCV to reach the best model.

# Code and Resources used
-Python Version: 3.7
-Packages: Pandas, Numpy, Sklearn, Matplotlib, Seaborn, 

# Data Cleaning
I needed to clean the data so that it can be used for my model. I made the foloowing changes and created the following variables
-Parsed numeric data out of salary 
-Made columns for employer provided salary and hourly wages
-Removed rows without salaries
-Created new column for company state
-Created columns for different skills
  Python
  SQL
  AWS
  Excel
-COlumn for simplified job titles and seniority

# Exploratory Data Analysis
I looked at the distributions of the data and the value counts for various categorical values. Here are few highlights 

![alt text](https://github.com/jay7Kumar/GlassDoor_Salary_Model/blob/main/Screenshots/Screenshot%202023-03-05%20at%206.03.12%20PM.png)
![alt text](https://github.com/jay7Kumar/GlassDoor_Salary_Model/blob/main/Screenshots/Screenshot%202023-03-05%20at%206.02.24%20PM.png)
![alt text](https://github.com/jay7Kumar/GlassDoor_Salary_Model/blob/main/Screenshots/Screenshot%202023-03-05%20at%206.03.28%20PM.png)
![alt text](https://github.com/jay7Kumar/GlassDoor_Salary_Model/blob/main/Screenshots/Screenshot%202023-03-05%20at%206.04.14%20PM.png)
![alt text](https://github.com/jay7Kumar/GlassDoor_Salary_Model/blob/main/Screenshots/Screenshot%202023-03-05%20at%206.04.45%20PM.png)

# Model Buillding
I transformed the categorical variables into dummy variables. I split the data into train and test sets witha test size of 20%
I tried three different models and evaluated them using Mean Absolute Error. I chose Mean Absolute Error because it is easy to iterpret and outliers arent particularly that bad
-Multiple Regression : baseline for thr model
-Lasso Regression : because of the sparse data from many categorical variables. I thought a normalized regression like Lasso will be effective
-RandomForest Regression : due to sparsity of the data , I thought this would be a good model
