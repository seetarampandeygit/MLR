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

## Data understanding, preparation and EDA
- Understanding DataFrame and structure of the data set (Headers, shape, info, columns data type, date formatting)
- Renaming columns to have meanings
- Checking distribution of our target variable 'total_rentals'
- Mapping the values of variables 'season', 'weather_type', 'weekday' and 'month' for better undertanding of numerical codes
- Dropping Irrelevant Columns
- Categorical Varaible Anylysis
- Creating Dummy Variables to represent different categorical variables as 0 and 1 so that could be included in our linear regression model if needed
- Analysing Numerical Variables

## Linear Regression Model Building and Evaluation
- Dropping Irrelevant columns
- Splitting our 'day' DataFrame in 'train' and 'test' set
- Analyse basic properties of train set
- Scaling
- Build model using RFE (Recursive Feature Elimination)
- Creating different LR models (if needed) after checking p-values, R^2, adj R^2, F-statistics and VIF and then dropping the insignificant variable
- Residual Analysis
- LR Assumptions Validation
- Making predictions or drawing inferences (from Test set)
- y_test vs.y_test_predicted
- Test_set R^2 and adj R^2

## Conclusions (Major)
- Assumptions of Linear Regression are satisfied
- Temperature influences the Bike rentals the most. The higher the temperature, the more are the rentals. This means a unit change in temperature keeping other variables fixed would spur the demand for rental bikes by approx. 42.8%. This was the same inference we drew from EDA.
- The business concept is gaining popularity. Even if all other factors are taken away, still the business will grow by about 24.5% year by year keeping the other features fixed.
- Light Snow and Light Rain affect Bike rentals the most in a negative way. This means a unit change in Snow and Rain attributes keeping other variables fixed would discourage the demand for rental bikes by approx. 28.9%. (Same inference from EDA)
- During the spring season bike rentals are less (same inferences by EDA).
   

  
## Acknowledgements

- This project was inspired by ML-AI couse at UpGrad and IIIT-B
- References: UpGrad and IIIT-B
- This project was based on [Linear Regression Assignment]([https://learn.upgrad.com/course/5811/segment/57681/345226/1043364/5213120]).


## Contact
Created by [@seetarampandeygit]  - feel free to contact me!
