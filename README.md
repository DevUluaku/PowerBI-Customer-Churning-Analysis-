# Customer Churn Analysis – Power BI Dashboard (Databel Telecom)

## Overview
This Power BI project explores customer churn for Databel, a fictional telecom provider.it is made up of a single data table containing 29 columns, and each row represents a customer, it has a churned column indicating if a customer has churned or not. The goal is to identify key drivers of customer churn and provide actionable insights that could help the company improve retention strategies.

## Data
- **Source**: Fictional customer dataset
- **Attributes**: Customer Status, Customer demographics, contact information, subscription types & charges, and churn status.
- **Size**: ~6687 records

## Objectives
- Understand which customer segments are most likely to churn
- Uncover patterns in churn behavior based on usage and demographics
- Present insights with interactive visualizations
- **Preprocessing**:  Using Power Query – I checked for duplicates and missing values, there were no duplicates or missing values except in churn reason and churn category which are linked to customers who didn’t churn.
Next is to check for distinct values in the CustomerID column which showed that distinct values match the unique values, meaning the CustomerID columns contains unique values.

## Methodology
- **Power Query**: Cleaned and transformed the dataset for consistency
- **DAX Measures**: Built key metrics like:
Number of Customers: COUNT(‘Databel-Data’[Customer ID]
Churned: IF(‘Databel-Data’[Churn Label]= “Yes”, 1,0)
Number of churned customers
  - Churn Rate:
  
- **Visualizations**:
  - Pie charts for churn distribution
  - Bar charts for churn by demographics (age group, gender, contract type)
  - Filters to slice data by customer type, tenure, and payment method

## General Insights
1.	Competitors are the main reasons for churning.
2.	Senior Citizens are more likely to churn than younger customers.
3.	CA has the highest churn rate but the lowest number of customers.
4.	DC has the lowest churn rate and out of the churned 11 was as a result of competitors.
5.	Customers on month-to-month plans had the highest churn rates.
6.	Length of a customer account is inversely proportional to the churn rate.
7.	There’s no discernable connection between churn rate and gender.





