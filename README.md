# BoomBikeSharing Case Study

This Multiple Linear Regression study seeks to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Dataset Reading](#dataset-reading)
* [Data Cleaning](#data-cleaning)
* [Data_Filtering](#data-filtering)
* [Data Standardization](#data-standardization)
* [Univariate Analysis](#univariate-analysis)
* [Bivariate Analysis](#bivariate-analysis)
* [Derived Metrics](#derived-metrics)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- This is a programming assignment in which we build a multiple linear regression model to predict the demand for shared bikes.
  
- A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short-term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock in the same system.
- A US bike-sharing provider, BoomBikes, has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company finds it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
- In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.
- They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know: • Which variables are significant in predicting the demand for shared bikes? • How well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.
   
- The aim is to model the demand for shared bikes with the available independent variables
  
- We utilized the dataset referred to as 'day.csv'. It includes information related to Bike rentals 'year-wise', 'season_wise', 'Weather_type_wise', 'different temperature redings of 730 days', 'working_day', 'holdiday'.


## Technologies Used
- numpy - version 1.26.4
- matplotlib - version 3.8.4
- seaborn - version 0.13.2
- pandas - version 2.2.2
- scikit-learn (or sklearn): 1.4.2
- statsmodels: 0.14.2

## Dataset Reading
- Headers and Top-5 rows
- Shape
- Index Range and Column's datatype

## Data Cleaning
- Null values processing

## Data Filtering
- Data Duplicacy Check
- Segragating and Analysing variable type (Categorical, Numerical)

## Data Standardization
- Converting variables 'int-rate' and 'revol_util' to numeric

## Univariate Analysis
### Numerical Variables
- Loan Amount Distribution
- Interest Rates
- Revolving Utilities
- Installments
### Categorical Variables
- Unique Member Check
- Loan Term
- Customer Grade
- Employment Length
- Verification Status
- Loan Purpose
- Home Ownership

## Bivariate Analysis
- Loan Term Vs Loan Status
- Grade vs Loan_status
- Subgrade Vs Loan_Status
- Purpose vs Loan_Status
- Employment Length Vs Loan_Status
- House Ownership Vs Loan Status

## Derived Metrics
- emp_len&Term vs loan status
- purpose&emp_len vs loan status
- credit_enquiry vs loan status
- public_record vs loan status
- bankruptcy vs loan status
- delinq_record vs loan status
- perc_util vs loan status
- interest vs loan status
- dti_buck vs loan status

## Conclusions
- Institution Loss: Typically, around 14% to 15% of members default, which is quite significant.
  
- Loan Term: The organization offers a 36-month loan repayment period for approximately 78% of its clients. However, customers with a 60-month loan repayment term are generally more prone to default. This was further confirmed when analyzed alongside the length of employment. Regardless of how long a customer has been employed, those with a 60-month tenure have a greater likelihood of defaulting. Therefore company should have a stringent policy to minimize lending for 60 months tenure.

- Customer Grade: Most customers fall into grades A or B. However, those in grades G, F, and E have a higher probability of defaulting. Therefore, the company should refrain from extending loans to customers in grades G, F, and E.

- Purpose of Loan: The company should be wary or exercise additional caution when providing loans for small business ventures or renewable energy projects, as these are more prone to default. This was further confirmed when analyzed in conjunction with the length of employment.

- Customer Collateral: It is noted that individuals whose home ownership status is labeled as unknown (other) tend to have a higher likelihood of default. The company should make sure to obtain appropriate collateral guarantees before providing loans.

- Credit History: The company needs to exercise extreme caution when lending to customers who have any credit inquiries within the past six months, those with any public record entries, or individuals with a history of bankruptcy.

- Customer Behaviour: The company should also make sure to review the delinquency history of a customer for at least two years before issuing loans. The analysis indicated that individuals with any delinquency history are more likely to default.

- Customer Financial Situation: The organization needs to thoroughly evaluate the Debt-to-Income (DTI) ratio before making decisions on loan approvals or setting interest rates. The interest rates should not be excessively high. It has been noted that as both the DTI and interest rates rise, the likelihood of default also escalates.

- Customer Credit Limit: Customers who make greater use of credit lines are at a higher risk of default. Consequently, the company should focus on this significant variable as well.

- Institution Research: The lending institution has failed to consider crucial factors before granting loans. It appears that there is almost no correlation between aspects such as bankruptcy records and loan amounts, debt-to-income ratios and loan amounts, delinquency records and loan amounts, and so forth.

  
## Acknowledgements

- This project was inspired by ML-AI couse at UpGrad and IIIT-B
- References: UpGrad and IIIT-B
- This project was based on [Exploratory Data Analysis]([https://learn.upgrad.com/course/5811/segment/53276/316330/957989/4783435]).


## Contact
Created by [@seetarampandeygit]  - feel free to contact me!
