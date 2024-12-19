# Zomato Insights: Analysing Popular Restaurants in India

![image](https://github.com/user-attachments/assets/11bed77f-fbfa-4dc7-82cf-89c11dc7f403)


## Introduction
Zomato is India's largest online platform offering comprehensive information, menus, and user reviews of restaurants across various venues. It helps users select the perfect dining spot by providing detailed insights into restaurant offerings, diverse cuisines, taste preferences, and other viable options. This Kaggle dataset comprises a collection of restaurants registered on Zomato in Bengaluru City. The dataset contains over 50,000 rows and 17 columns, offering a wealth of information to explore. By cleaning, transforming, analysing, and visualising the data, the aim is to delve into Zomato's extensive database to uncover hidden patterns, analyse customer behaviors, and identify trends reflecting the evolving tastes of Indian consumers.


## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Analysis](#analysis)
- [Results](#results)
- [Visualisation](#visualisation)


## Features
### Feature 1: name
Name of the restaurant in the dataset.

### Feature 2: online_order
This is a categorical variable with two responses: 'Yes' and 'No.' It indicates whether a restaurant accepts online orders.

### Feature 3: book_table
This is a categorical variable with two responses: 'Yes' and 'No.' It indicates whether a restaurant accepts table bookings.

### Feature 4: rate
Initially in the dataset, this is a categorical variable formatted as 'x.x/5.0.' It represents the customer rating for the restaurant on a scale of 5.0. It should be converted to a numerical type for analysis.

### Feature 5: rest_type
This is a categorial variable representing the restaurant type.

### Feature 6: cuisines
This is a categorical variable that represents a list of a restaurant's cuisines. Each restaurant may offer more than one cuisine.

### Feature 7: approx_cost(for two people)
Initially, this is a categorical variable in the dataset that represents the approximate cost for two people at each restaurant. It should be converted to a numerical type for analysis.

### Feature 8: listed_in(city)
This is a categorical variable representing the location of the restaurant.


## Analysis
### Data Cleaning
- Identify and remove duplicate rows from the dataset to ensure data integrity.
- Identify redundant columns and drop them
- Handle missing values by:
  - Numerical Features: Fill missing values with the mean of the respective column.
  - Categorical Features: Fill missing values with the placeholder value "Unknown."
  - Feature with Few Missing Values: Drop rows containing missing values if the missing values in that feature account for less than 5% of the dataset.

### Exploratory Data Analysis (EDA) and Data Visualisation
- Analyse each feature to identify trends and patterns. Use appropriate visualisations such as:
  - Pie Chart: For categorical features like online order and book table.
  - Histogram: To understand the distribution of numerical features like ratings or costs.
  - Bar Chart: For comparing categories, e.g., the number of restaurants by location or cuisine.
- Explore the correlation between each feature by plotting:
  - Between Numerical Feature and Categorical Feature: Box Plot, Bar Chart
  - Between 2 Numerical Features: Scatter Plot, Heat Map
- Identify top performing restaurant chains, restaurant types, and cuisines.
- Some business questions to explore:
  - Which types of restaurants are most likely to offer online order and table booking?
  - Are there cuisines that have high ratings but relatively few restaurants, indicating a market opportunity to expand those offerings?
  - What common characteristics do the top 10% of restaurants (by rating) share?
  - Which cuisines have the highest average rating, and what does that say about customer preferences?


## Results
- Cuisine Trends: Identified some popular cuisines such as North Indian, Chinese, and Cafe.
- Top Restaurant Types: Microbrewery & Casual Dining is the best restaurant type with an average rating of more than 4.3.
- Outstanding characteristics of the top 10% highest-rated restaurants:
  - They are more likely to accept table bookings.
  - Casual Dining, Bar, and Pub are popular restaurant types among the top 10%.
  - These restaurants generally have a higher price range compared to those outside the top 10%.
  - They are frequently located in bustling commercial centers where high-end dining experiences are sought after.
- Opportunity cuisines: Certain cuisines, such as Cantonese, African, and Malaysian, have exceptionally high ratings but are represented by a relatively small number of restaurants, indicating potential opportunities for growth and market expansion.


## Visualisation
Tableau interative dashboard is available to explore more about the data insights: https://public.tableau.com/shared/Y2PYDT2BB?:display_count=n&:origin=viz_share_link
