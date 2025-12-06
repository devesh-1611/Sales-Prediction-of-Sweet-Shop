# Sweet Shop Sales Analysis (2020–2025) & Forecasting Project
This project performs an end-to-end data analysis, visualization, festival-wise performance study, and machine-learning-based sales forecasting for a Sweet Shop using data from 2020 to Nov 2025.

The analysis includes:

 Complete EDA
 Festival-wise sales insights (Diwali, Rakshabandhan, Sankranti)
 Weekend vs Weekday behavior
 Month-wise & Week-wise performance
 Product-wise & Branch-wise breakdown
 ML Forecasting using Random Forest, XGBoost, and Custom RandomForest
 Generating 365-day future sales prediction per product

Project Overview

This project focuses on analyzing Sweet Shop sales data to identify:

Seasonal and festival patterns

Customer buying behavior across weekdays vs weekends

Fast-moving products and high-performing branches

Long-term trends (monthly and weekly)

Future forecasts for business planning

The final output includes detailed plots + a CSV file containing product-wise 365-day future sales predictions.



Technologies Used
Category	Tools
Language	Python 3
Data Manipulation	pandas, numpy
Visualization	matplotlib, seaborn
Modeling	scikit-learn, XGBoost
Forecasting	RandomForestRegressor, custom RandomForest
File I/O	Excel reading, CSV Export



Columns (typical):

Date

Product

Qty

TotalAmount → renamed to Sales

Branch

Other metadata

. Data Preprocessing & Feature Engineering

Performed steps:

 Data Inspection

df.head()

df.info()

Shape, missing values, duplicates

Festival-Wise Sales Insights

The project analyzes key Indian festivals:

 Diwali (Oct–Nov)

Year-wise Diwali week sales extracted using predefined date ranges.

 Rakshabandhan (August)

Both full-month & Rakhi-week sales calculated.

 Sankranti (January)

Month-wise and Sankranti-week sales evaluated

6. Visual Analysis
 Weekend vs Weekday Sales (Pie Chart)

Shows contribution of weekends in total revenue.

 Month-wise Sales Trend (Line Plot)

Identifies high-performing months.

 Week-wise Sales Trend (Bar Plot)
 Product-wise Sales (Bar Plot)
 Branch-wise Sales (Bar Plot)

All visualizations use seaborn & matplotlib

Machine Learning for Forecasting
Feature Encoding

Branch encoded

Product encoded

Models Used
 Custom RandomForest Implementation (Baseline Model)

Trains 10 “dummy” trees

Predicts mean sales

MAE & R² evaluated

 RandomForestRegressor for 365-Day Forecast

Trained per product

Predicts next year’s sales for every product

XGBoost Regressor

Compared MAE & R² with custom RandomForest

Usually more accurate

. Forecasting Output

For each product:

Historical + Predicted data combined

Future 365-day forecast generated

Individual prediction plots generated

Saved to CSV for reporting

Author

Devesh Sharma
