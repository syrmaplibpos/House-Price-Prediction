# House-Price-Prediction

## Background

Ames is a city in Iowa, United States, located approximately 560 km from Chicago.
It is best known as the home of Iowa State University (ISU).
As of 2021, more than 30,708 students enrolled in ISU.
The top 1 employer in the city is ISU with 16,647 employees.

## Business Challenges And Objectives 

### Challenges

With pandemic restrictions easing across the United States, students and employees are getting back to school. 
Further, in the wake of the pandemic, 62% of views from Realtor.com’s online searches were for houses in the suburbs compared to 38% in urban areas (Learner, 2022).

### Objectives

Investigate what important features would affect house prices.
Train a prediction model and help people to make better decisions when it comes to home investment. 

## 1. Business Understanding
A house purchase is most likely the largest financial decision a person, couple or family will make in their lifetime. Approximately 66% of urban adults with lower household incomes say affordable housing in their urban areas is a major problem (Schaeffer, 2022).  Further, in the wake of the pandemic, 62% of views from Realtor.com’s online searches were for properties in the suburbs compared to 38% in urban areas (Lerner, 2022). It implies that home buyers will continue to have a preference for the suburbs. To gain a better understanding of the housing market in suburbs, we want to investigate what important features would affect house prices.
We found a raw dataset that describes every aspect of residential homes in Ames, Iowa from Kaggle, which enables us to dig into the variables in depth and to provide a model that could more accurately estimate house prices. In this way, people could make better decisions when it comes to home investment. 

## 2. Data Understanding & Preparation 
We have two datasets: training set and test set. Datasets are collected from [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview/description). The training set is designated to train our prediction models, consisting of 81 columns with sale prices column and 1,460 rows. The test set is designated to test trained models, consisting of 80 columns without sale price column and 1,459 rows. The datasets have 37 numeric variables and 43 categorical variables. 

Before diving into the data cleaning process, let us to see the sale prices distribution in Ames city to better understand the target variable. From figure 2.1, most people are willing to spend around $200,000 for housing. Only a small portion of consumers can afford expensive houses in Ames. 
We combined train and test datasets by rbind() function to manipulate data cleaning for higher efficiency. There is a total of 35 predictor variables, 12 numeric variables and 23 categorical variables, that have missing values. We replaced the missing values with the number “zero” if it is numeric. We replaced the missing values with the text “none” if it is categorical. Once all missing values were removed, the next step was to convert character variables into ordinal integers using revalue() function if there is clear ordinality. Otherwise, we converted character variables into a factor data type.

After data preprocessing, the number of numeric variables was increased from 37 to 56. We used cor() function to calculate the correlation between predictor variables and sale price, and selected only high correlation (correlation > 0.5). From figure 2.2, we see that 16 predictor variables were selected and would be used for modeling in next section.

## Data Collection

Two datasets

The training set: a subset to train a model. The test set: a subset to test a trained model 

Datasets are collected from [Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview/description)

## Data Preprocessing

### Data Integration

rbind( ) function to combine train and test datasets by rows.

### Data Cleaning

is.na( ) to identify columns that have NAs. Replace it with number zero or text none

## Data Transformation

Convert character variables into ordinal integers  using revalue( ) function if there is clear ordinality. Otherwise, convert them into factor

## Feature Selection

Most people are willing to spend 200,000 for housing. Only small proportion of consumers can afford expensive houses in Ames. 

Select only high correlation with Sale Price (correlation > 0.5) 

## Modeling
Multiple Linear Regression, CART, Random Forest

## Result & Evaluation

## References

[https://www.washingtonpost.com/business/2021/12/23/suburbs-still-hotter-than-cities-home-buyers](https://www.washingtonpost.com/business/2021/12/23/suburbs-still-hotter-than-cities-home-buyers)

[https://www.zillow.com/research/data/](https://www.zillow.com/research/data/)

[https://www.kaggle.com/code/bluedreamv1b3/house-price/notebook](https://www.kaggle.com/code/bluedreamv1b3/house-price/notebook)

[https://www.kaggle.com/code/erikbruin/house-prices-lasso-xgboost-and-a-detailed-eda](https://www.kaggle.com/code/erikbruin/house-prices-lasso-xgboost-and-a-detailed-eda)

[https://www.kaggle.com/code/shaoyingzhang/data-exploration-and-prediction-of-house-price](https://www.kaggle.com/code/shaoyingzhang/data-exploration-and-prediction-of-house-price)















