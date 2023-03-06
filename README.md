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
