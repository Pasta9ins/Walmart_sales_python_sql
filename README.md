# Walmart Data Analysis: End-to-End SQL + Python

## Project Overview

![Project Pipeline](https://github.com/najirh/Walmart_SQL_Python/blob/main/walmart_project-piplelines.png)

This project is an end-to-end data analysis solution designed to extract critical business insights from Walmart sales data. We utilize Python for data processing and analysis, SQL for advanced querying, and structured problem-solving techniques to solve 17 key business questions. The project is ideal for data analysts looking to develop skills in data manipulation, SQL querying, and data pipeline creation.

---

## Project Steps

### 1. Set Up the Environment
   - **Tools Used**: Visual Studio Code (VS Code), Python, SQL (MySQL and PostgreSQL)
   - **Goal**: Create a structured workspace within VS Code and organize project folders for smooth development and data handling.

### 2. Downloading Raw Walmart Sales Data
   - **Data Source**: Use the Kaggle API to download the Walmart sales datasets from Kaggle.
   - **Dataset Link**: [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)
   - **Data Structure**: 9,969 transactions across 12 columns including invoice details, branch information, product categories, pricing, customer ratings, and payment methods.

### 3. Installing Required Libraries and Load Data
   - **Libraries**: Install necessary Python libraries using:
     ```bash
     pip install pandas numpy sqlalchemy mysql-connector-python 
     ```
   - **Loading Data**: Read the data into a Pandas DataFrame for initial analysis and transformations.

### 4. Explore the Data
   - **Goal**: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
   - **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.
   - **Key Findings**: Identified 12 columns with mixed data types requiring cleaning and standardization.

### 5. Data Cleaning
   - **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
   - **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
   - **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
   - **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
   - **Validation**: Check for any remaining inconsistencies and verify the cleaned data.

### 6. Feature Engineering
   - **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
   - **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 7. Load Data into MySQL and PostgreSQL
   - **Set Up Connections**: Connect to MySQL and PostgreSQL using `sqlalchemy` and load the cleaned data into each database.
   - **Table Creation**: Set up tables in both MySQL and PostgreSQL using Python SQLAlchemy to automate table creation and data insertion.
   - **Verification**: Run initial SQL queries to confirm that the data has been loaded accurately.

### 8. SQL Analysis: 17 Complex Business Problems and Solutions
   - **Business Problem-Solving**: Write and execute 17 comprehensive SQL queries to answer critical business questions across multiple domains:

#### Payment & Transaction Analysis (Q1, Q4, Q7, Q11, Q13)
- Payment method performance and transaction volumes
- Customer spending patterns by payment type
- Payment method preferences across branches
- Satisfaction correlation with transaction values

#### Performance & Ratings Analysis (Q2, Q5, Q12, Q14, Q16)
- Highest-rated categories by branch
- Rating distribution across cities and categories
- Profit margin optimization opportunities
- Branch performance comparison with market share
- Customer segmentation based on spending behavior

#### Time-Based Analysis (Q3, Q8, Q15, Q17)
- Busiest days for each branch
- Sales performance across morning, afternoon, and evening shifts
- Peak profitability time slots
- Operational efficiency and resource allocation

#### Revenue & Profit Analysis (Q6, Q9, Q10)
- Total profit calculation by category
- Year-over-year revenue comparison
- High-value vs low-value transaction characteristics

#### Advanced Analytics (Q14, Q15, Q17)
- Geographic performance analysis
- Market share calculations
- Operational efficiency metrics

## Business Insights Discovered

### Sales Performance Insights
- **Payment Methods**: Identified preferred payment methods by branch and their correlation with transaction values
- **Time Patterns**: Discovered peak sales hours and optimal time slots for maximum profitability
- **Geographic Analysis**: Market share distribution across branches and cities

### Customer Behavior Analysis
- **Segmentation**: Customer spending patterns categorized into Premium, High-Value, Medium-Value, Standard, and Budget segments
- **Satisfaction Metrics**: Correlation between customer ratings and transaction values
- **Behavioral Trends**: Shopping patterns across different time periods and categories

### Operational Efficiency
- **Resource Allocation**: Identified branches and time periods requiring better staffing
- **Performance Metrics**: Transaction processing efficiency and customer satisfaction correlation
- **Profit Optimization**: Categories with high margins but low volume indicating growth opportunities

### Revenue & Profitability
- **Category Performance**: Most and least profitable product categories
- **Year-over-Year Analysis**: Revenue trends and performance comparisons
- **Margin Analysis**: Profit margin optimization opportunities

## Technical Achievements

- **Advanced SQL Techniques**: Implemented CTEs, Window Functions, Ranking, and Complex Joins
- **Data Pipeline**: Complete ETL process from raw data to actionable insights
- **Cross-Database Compatibility**: Queries optimized for both MySQL and PostgreSQL
- **Scalable Analysis**: Structured approach enabling easy addition of new business questions

## Future Enhancements

Possible extensions to this project:
- **Dashboard Integration**: Connect with Power BI or Tableau for interactive visualization
- **Real-Time Analytics**: Automation of the data pipeline for live data ingestion
- **Predictive Modeling**: Machine learning models for sales forecasting and customer behavior prediction
- **Additional Data Sources**: Integration of inventory, customer demographics, and external market data
- **Advanced Analytics**: A/B testing frameworks and recommendation systems

---

**Project Status**: ✅ Complete - 17 Business Problems Solved with Advanced SQL Analysis

---

## ©️ License & Credits

- © 2025 **Anirudha Chaudhary**. All rights reserved.

---

## 🙌 Made with ❤️ by **Anirudha Chaudhary**
