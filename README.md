Credit Card Transaction Analysis 💳

Project Overview

This project performs a comprehensive analysis of credit card transactions to understand spending patterns, customer demographics, and regional trends. Using Advanced SQL, I analyzed a dataset comprising credit card transaction records to extract actionable business insights.

The goal was to solve real-world business questions regarding customer spending behavior, such as identifying high-value locations, analyzing month-over-month growth, and detecting specific milestones in card usage.

🗂 Database Schema

The analysis is based on the credit_card_transactions table with the following structure:

transaction_id: Unique identifier for each transaction

city: City where the transaction occurred

transaction_date: Date of transaction

card_type: Type of card (Gold, Silver, Platinum, etc.)

exp_type: Type of expense (Bills, Food, Fuel, Entertainment, etc.)

gender: Gender of the cardholder

amount: Transaction amount

🛠 Tech Stack

Database: MS SQL Server (T-SQL)

Key SQL Concepts Applied:

Common Table Expressions (CTEs): For readable and modular code.

Window Functions: RANK(), ROW_NUMBER(), LAG(), SUM() OVER().

Date Manipulation: DATEPART, DATEDIFF for time-series analysis.

Conditional Aggregation: CASE WHEN statements for pivoting data.

Subqueries & Joins: For complex filtering and data retrieval.

📊 Business Problems Solved

This repository contains SQL queries addressing the following 9 key business questions:

Top 5 Cities by Spend: Identifying the highest contributing cities and their percentage share of total transaction volume.

Highest Spending Months: Finding the peak spending month and amount for each specific card type.

Cumulative Spend Milestones: Retrieving transaction details for the exact moment each card type reached a cumulative spend of 1,000,000.

Gold Card Usage: Identifying the city with the lowest percentage of spend contributed by Gold card users.

Expense Extremes: determining the highest and lowest expense types for each city.

Demographic Insights: Calculating the percentage contribution of female spenders across different expense categories.

MoM Growth Analysis: Identifying which card and expense type combination saw the highest Month-over-Month growth in Jan 2014.

Weekend Spending Patterns: Finding the city with the highest average spend per transaction during weekends.

Transaction Velocity: Identifying which city took the least number of days to reach its 500th transaction.

💡 Key Insights (Example)

Note: These insights are derived from the query outputs.

Growth Trends: Analysis of MoM growth helps identify emerging spending categories.

City Tiers: The ratio of transactions to spend helps distinguish between high-volume/low-value cities and low-volume/high-value cities.

Customer Segmentation: Gender and Card Type breakdowns allow for targeted marketing strategies.

🚀 How to Run

Import Data: Load the dataset into your SQL Server environment.

Run Queries: Execute the .sql script file in this repository.

Verify Results: Check output against expected business logic.

Author: Shashwat Vashisht
Connect with me on LinkedIn (https://www.linkedin.com/in/shashwat-vashisht-0019b2255/)
