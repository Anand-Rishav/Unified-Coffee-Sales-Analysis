# Unified Coffee Sales Analysis

## Overview

Unified Coffee Sales Analysis is a comprehensive project designed to analyze transactional data from a coffee vending machine. The primary goals are to uncover sales trends, understand customer behavior, and generate forecasts to optimize inventory and marketing strategies. By leveraging modern Python data science libraries and statistical modeling, this repository delivers actionable insights for business decision-making in the beverage sector.

---

## Dataset

The analysis is centered on the `coffee.csv` dataset, which records every transaction with the following fields:
- **date:** Date of transaction
- **datetime:** Exact timestamp for each purchase
- **cash_type:** Payment method (card or cash)
- **card:** Anonymized card identifier (used for card payments)
- **money:** Transaction amount
- **coffee_name:** Type of coffee purchased

---

## Analysis Workflow

The project follows a robust, step-by-step approach:

### 1. Data Loading & Preprocessing

- **Inspection:** Read and examine raw data for integrity.
- **Type Conversion:** Convert string-based dates and times to datetime objects.
- **Missing Value Handling:** Address missing values, especially in the `card` column, to clarify cash/card payments.
- **Feature Engineering:** Extract relevant features such as hour of day, day of week, and aggregate customer statistics.

### 2. Exploratory Data Analysis (EDA)

- **Popular Products:** Identify best-selling items (Latte and Hot Chocolate lead in both sales and revenue).
- **Revenue Analysis:** Reveal which products generate the most income.
- **Temporal Patterns:** Pinpoint peak sales hours (usually lunch, 12–2 PM) and examine sales across weekdays and weekends.
- **Payment Method Trends:** Highlight the dominance of card payments over cash.
- **Seasonality:** Analyze weekly cyclic trends and weekend dips in sales.

### 3. Customer Behavior Analysis

- **Top Customers:** Rank buyers by purchase frequency and spending.
- **Preference Mining:** Uncover individual coffee preferences and customer loyalty patterns.

### 4. Time Series Forecasting

- **Modeling:** Use the Prophet library to forecast daily sales.
- **Trend Detection:** Capture underlying trends and weekly seasonality.
- **Prediction:** Provide actionable forecasts for the next day, week, and month to support planning and inventory decisions.

---

## Data Visualization & Analysis Techniques

- **Data Cleaning:** Remove inconsistencies and prepare data for analysis.
- **GroupBy and Aggregation:** Summarize sales by product, payment method, hour, weekday, and customer.
- **Bar Charts & Time Series Plots:** Visualize product popularity, sales trends, and seasonality.
- **Heatmaps:** Reveal temporal patterns in sales across hours and days.
- **Statistical Summaries:** Provide descriptive statistics for revenue and transaction counts.

---

## Python Libraries Used

Typical libraries (based on standard data analysis workflows and the use of Prophet):
- **pandas:** For data manipulation and aggregation
- **numpy:** For numerical operations
- **matplotlib / seaborn:** For plotting and data visualization
- **Prophet:** For time series forecasting
- **datetime:** For handling date and time features

---

## Key Insights

- **Product Focus:** Latte and Hot Chocolate drive sales volume and revenue.
- **Sales Timing:** Weekday lunch hours are critical for promotions and inventory.
- **Customer Preference:** Card payments dominate, suggesting the need for fast, digital checkout.
- **Seasonal Patterns:** Predictable weekly cycles and weekend dips inform staffing and stocking.
- **Forecasting Value:** Data-driven forecasts aid in proactive inventory management and business planning.

---

## Repository Structure

- `coffee.csv`: Core transaction dataset
- `Coffee Sales Notebook.ipynb`: Jupyter notebook containing all scripts for data loading, preprocessing, EDA, customer segmentation, and forecasting
- `README.md`: Comprehensive project documentation

---

## Getting Started

To reproduce the analysis or modify it for your own data:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Anand-Rishav/Unified-Coffee-Sales-Analysis.git
   ```

2. **Set Up Python Environment:**  
   Create and activate a virtual environment (recommended).
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install Required Packages:**  
   Typical installations include:
   ```bash
   pip install pandas numpy matplotlib seaborn prophet
   ```

4. **Run the Notebook:**  
   Use Jupyter or VS Code to open and execute `Coffee Sales Notebook.ipynb`.

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Contact

For questions, feedback, or contributions, please open an issue or reach out via GitHub.

---
