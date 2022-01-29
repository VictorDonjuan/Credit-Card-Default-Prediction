See the full project in the Jupyter Notebooks:



# Predicting Credit Card Default Project: Overview

In this problem, we will explore the [public dataset](http://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) that comes from a credit card company. The excel file consists of 30,000 observations, 23 features and 1 response variable. The attribute information is explained in the following way:

"This research employed a binary variable, default payment (Yes = 1, No = 0), as the response variable. This study reviewed the literature and used the following 23 variables as explanatory variables:"
- X1: Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit.
- X2: Gender (1 = male; 2 = female).
- X3: Education (1 = graduate school; 2 = university; 3 = high school; 4 = others).
- X4: Marital status (1 = married; 2 = single; 3 = others).
- X5: Age (year).
- X6 - X11: History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows: X6 = the repayment status in September, 2005; X7 = the repayment status in August, 2005; . . .;X11 = the repayment status in April, 2005. The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.
- X12-X17: Amount of bill statement (NT dollar). X12 = amount of bill statement in September, 2005; X13 = amount of bill statement in August, 2005; . . .; X17 = amount of bill statement in April, 2005.
- X18-X23: Amount of previous payment (NT dollar). X18 = amount paid in September, 2005; X19 = amount paid in August, 2005; . . .;X23 = amount paid in April, 2005.

# The Problem, Data Analysis and Data Cleaning

A default occurs when a borrower is unable to make timely payments or misses payments. In this case, 30,000 observations in the dataset come along some demographic features as well as the last 6 months behaviours regarding their payments, whether they have defaulted before or the amount of bill statements they had to pay. The response variable, namely the variable we want to predict, 'default payment next month', indicates wheter or not an account owner has defaulted the following month (1 = defaulted, 0 = did not default).

Although this is a binary classification problem, the response variable is highly unbalanced since more people do tend to make timely payments. 

![alt text](count_default.JPG "Title")
