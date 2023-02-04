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

## Modeling 1 Time Series Analysis

## Modeling 2 Multiple Linear Regression

## Modeling 3 CART

## Modeling 4 Random Forest

## Result & Evaluation

## References

[https://www.washingtonpost.com/business/2021/12/23/suburbs-still-hotter-than-cities-home-buyers](https://www.washingtonpost.com/business/2021/12/23/suburbs-still-hotter-than-cities-home-buyers)

[https://www.zillow.com/research/data/](https://www.zillow.com/research/data/)

[https://www.kaggle.com/code/bluedreamv1b3/house-price/notebook](https://www.kaggle.com/code/bluedreamv1b3/house-price/notebook)

[https://www.kaggle.com/code/erikbruin/house-prices-lasso-xgboost-and-a-detailed-eda](https://www.kaggle.com/code/erikbruin/house-prices-lasso-xgboost-and-a-detailed-eda)

[https://www.kaggle.com/code/shaoyingzhang/data-exploration-and-prediction-of-house-price](https://www.kaggle.com/code/shaoyingzhang/data-exploration-and-prediction-of-house-price)















