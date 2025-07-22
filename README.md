Online Retail Sales EDA and Power BI Dashboard

This project performs exploratory data analysis (EDA) on a real-world e-commerce retail dataset and presents key insights using an interactive Power BI dashboard.

Dataset

Source: Online Retail II Dataset from Kaggle

Covers transactions from December 2010 to December 2011

Based on a UK online store

Format: Excel (.xlsx)

Key columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

Project Goals

Clean and preprocess the data

Perform univariate, bivariate, and multivariate analysis

Identify top-selling products, seasonal trends, and customer segments

Perform RFM segmentation

Visualize key insights using Power BI

Data Cleaning

Missing CustomerID values handled using mean imputation

Missing Description values handled using mode (most frequent item)

Removed duplicate rows

Removed cancelled orders (InvoiceNo starting with "C")

Removed or capped outliers in Quantity and UnitPrice using IQR method

Converted InvoiceDate to proper datetime format

Added TotalPrice column (Quantity × UnitPrice)

Exploratory Data Analysis (EDA)

General Overview:

Count of unique products, transactions, and customers

Country distribution of customers

Product Analysis:

Top 10 products by quantity sold

Top 10 revenue-generating products

Products with zero or negative unit prices

Customer Analysis:

Customers who bought the most items

Distribution of purchases per customer

Identification of loyal customers

Time Series and Trends:

Monthly revenue trend

Daily and weekly transaction patterns

Peak and slow sales seasons

Country Analysis:

Revenue by country

Number of orders per country

RFM Segmentation:

Recency: Days since last purchase

Frequency: Number of distinct invoices

Monetary: Total spending

RFM Score calculated using DAX in Power BI

Power BI Dashboard Features

Sales Overview

KPIs: Total Revenue, Number of Invoices, Unique Customers

Monthly Sales Trend (Line Chart)

Top Products

Top 10 products by quantity and revenue (Clustered Bar Chart)

Product breakdown using Treemap or Pie Chart

Customer Segments

RFM Table

RFM Scatter Plot

Top 10 Loyal Customers

Geographical Insights

Revenue by country using bar chart or map

Dashboard File: Online_Retail_Sales_Dashboard.pbix

How to Use This Project

Clone the repository

Open and run the Jupyter Notebook: Retail_EDA.ipynb

Export cleaned data as cleaned_retail_data.csv

Open Power BI Desktop and import the CSV

Build or view the dashboard using the .pbix file

Project Structure

cleaned_retail_data.csv

Retail_EDA.ipynb

Online_Retail_Sales_Dashboard.pbix

README.md

Tools Used

Python (Pandas, Matplotlib, Seaborn)

Jupyter Notebook

Microsoft Power BI

Excel

Author: Rashmeen Rehan  
GitHub: https://github.com/rashmeen74

