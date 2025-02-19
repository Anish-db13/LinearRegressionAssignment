# Linear Regression Assignment

**Problem Statement**

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 

**Business Goal:**

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

This project aims to analyze and predict bike rental demand based on various influencing factors such as weather conditions, seasonal effects, and holidays. By building a multiple linear regression model, we determine the key variables affecting bike rentals and evaluate the model's performance on training and test datasets.

### Background

Bike-sharing systems have gained popularity as an efficient and eco-friendly mode of transportation. Understanding the factors that influence bike demand can help optimize operations, improve availability, and enhance user experience.

### Business Problem

The project seeks to answer the following key business questions:
- What factors impact bike rental demand the most?
- Can we build a predictive model to forecast demand accurately?
- How well does the model generalize to unseen data?

### Dataset

The dataset used for this analysis contains information on bike rentals, weather conditions, seasonal effects, and holidays. The key variables include:

- Dependent Variable (Target): cnt (Total count of rented bikes)
- Independent Variables (Predictors):
  - `year` (Year of rental)
  - `holiday` (Whether the day is a holiday)
  - `temp` (Temperature in normalized form)
  - `windspeed` (Wind speed in normalized form)
  - `sep` (September flag)
  - `sat` (Saturday flag)
  - `Light_snowrain` (Indicator for light snow or rain)
  - `Misty` (Indicator for misty weather)
  - `spring` (Spring season flag)
  - `summer` (Summer season flag)
  - `winter` (Winter season flag)

## Conclusions

- The model achieved good performance with:
  - Training R²: 0.834, Adjusted R²: 0.830
  - Testing R²: 0.8042, Adjusted R²: 0.7939
- Key factors influencing bike demand include temperature, wind speed, seasonal changes (spring, summer, winter), and weather conditions (light snow/rain, misty weather).
- The presence of multicollinearity was checked using VIF values and a correlation heatmap, ensuring that independent variables do not have strong dependencies.

The model generalizes well but has some limitations due to external factors not captured in the dataset.
## Technologies Used

- Python - 3.x
- NumPy - 1.21.6
- Pandas - 1.3.5
- Matplotlib - 3.4.3
- Seaborn - 0.11.2
- Statsmodels - 0.13.2
- Scikit-learn - 1.0.2

## Acknowledgements

- This project was inspired by bike-sharing demand analysis use cases.
- Data used in this project was adapted from public datasets related to bike rental services.
- Special thanks to various statistical modeling and machine learning resources that guided the analysis.

## Contact
Created by [@anishdb13](https://github.com/anishdb13) - feel free to contact me!
