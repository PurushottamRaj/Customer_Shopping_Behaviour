# Customer_Shopping_Behaviour
Customer Shopping Behaviour Analysis examines 3,900 purchases across 18 features like demographics, purchase details, and behaviours. Python EDA cleaned data; SQL queried revenue, segments (New/Returning/Loyal), and discounts. Power BI dashboard offers insights for subscriptions, loyalty programs, and targeted marketing

Customer Shopping Behavior Analysis
This repository contains a comprehensive data analysis project examining customer shopping patterns from 3,900 transactions across multiple product categories. The analysis uses Python for data cleaning and exploration, SQL for business insights via PostgreSQL, and Power BI for visualization to derive actionable recommendations.​

Dataset Overview
Size: 3,900 rows, 18 columns

Key Features:
-Customer demographics: Age, Gender, Location, Subscription Status
-Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, Color
-Shopping behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type

Data Quality: 
-37 missing values in Review Rating (imputed using median per category)​

Analysis Pipeline
Python EDA
-Loaded data with pandas and performed initial exploration using df.info() and df.describe()
-Standardized columns to snake_case and engineered features like agegroup (binned ages) and purchasefrequencydays
-Dropped redundant promocodeused column after consistency checks
-Integrated with PostgreSQL by loading cleaned DataFrame into database​

SQL Queries (PostgreSQL)
-Key business questions addressed:
-Revenue comparison by gender
-High-spending discount users (above average spend)
-Top 5 products by average rating
-Shipping type vs. purchase amount (Standard vs. Express)
-Subscribers vs. non-subscribers (average spend and total revenue)
-Discount-dependent products (top 5 by % discounted purchases)
-Customer segmentation: New, Returning, Loyal (based on purchase history)
-Top 3 products per category
-Repeat buyers (5+ purchases) and subscription likelihood
-Revenue by age group​

Power BI Dashboard
-Interactive visualizations presenting key insights from SQL results for stakeholder review.​

Business Recommendations
-Promote subscription benefits to boost uptake
-Implement loyalty programs for repeat buyers
-Review discount policies to balance sales and margins
-Highlight top-rated/best-selling products in marketing
-Target high-revenue age groups and express shipping users​

Tech Stack
-Languages: Python, SQL
-Libraries/Tools: pandas, PostgreSQL, Power BI
-Files: shopping_behavior.csv (dataset), eda_notebook.ipynb, sql_queries.sql, powerbi_dashboard.pbix
