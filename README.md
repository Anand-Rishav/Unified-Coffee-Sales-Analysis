# Coffee Vending Machine Sales Analysis

## Project Overview

This project analyzes sales data from a coffee vending machine to uncover key trends, understand customer behavior, and forecast future sales. By leveraging data analysis and time series modeling, we aim to provide actionable insights for optimizing inventory, marketing strategies, and overall business decisions.

## Dataset

The analysis is based on the `coffee.csv` dataset, which contains detailed records of each transaction, including:
- **date**: Date of the transaction.
- **datetime**: Timestamp of the transaction.
- **cash_type**: Payment method (card or cash).
- **card**: Anonymized card identifier (for card payments).
- **money**: Transaction amount.
- **coffee_name**: Type of coffee purchased.

## Analysis and Findings

The analysis covered several key areas:

### Data Loading and Preprocessing
- Loaded and inspected the raw data.
- Converted date and datetime columns to appropriate formats.
- Handled missing values in the `card` column by identifying them as cash payments.
- Extracted time-based features like hour and day of the week.

### Exploratory Data Analysis (EDA)
- **Most Popular Products:** Latte and Hot Chocolate are the top-selling items.
- **Revenue Distribution:** Latte and Hot Chocolate also contribute the most to revenue.
- **Peak Sales Hours:** Sales peak during lunchtime (12 PM - 2 PM) and gradually decrease throughout the day.
- **Sales by Day of the Week:** Weekdays, especially Friday, have significantly higher sales than weekends.
- **Payment Method Preference:** Card payments are the dominant transaction type.
- **Daily Sales Trend:** Daily sales show a clear weekly seasonality.

### Customer Behavior Analysis
- Identified the top customers by purchase frequency and total spending.
- Analyzed individual customer preferences (e.g., the favorite coffee of the most frequent buyer).

### Sales Forecasting
- Utilized the Prophet library to model daily sales.
- The model captured the overall trend and weekly seasonality.
- Provided forecasts for the next 30 days, including predictions for the next day, week, and month.

## Key Insights

- Latte and Hot Chocolate are the primary drivers of both sales volume and revenue.
- Targeting promotions or ensuring sufficient stock during weekday lunch hours is crucial.
- Focusing on card payment options aligns with customer preferences.
- Strong weekly seasonality indicates predictable dips in sales on weekends.
- The forecasting model is a valuable tool for planning and inventory management.

## Repository Structure

- `coffee.csv`: The dataset used for the analysis.
- `Coffee Sales Notebook.ipynb`: Jupyter Notebook containing all code for data loading, preprocessing, EDA, customer analysis, and sales forecasting.
- `README.md`: Project overview and documentation.

---
