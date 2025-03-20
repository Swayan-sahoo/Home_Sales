# Home_Sales
# Home Sales Analysis with PySpark

## Project Overview

This project utilizes PySpark to analyze home sales data from an AWS S3 bucket. The dataset is loaded into a PySpark DataFrame, and SQL queries are executed to extract insights related to home pricing based on various criteria. Additionally, caching and partitioning techniques are implemented to optimize query performance.

Technologies Used

Python

PySpark (SparkSQL)

AWS S3

Jupyter Notebook

GoogleColab

Dataset

The dataset used for this project is home_sales_revised.csv, which contains information on home sales, including the number of bedrooms, bathrooms, floors, square footage, view ratings, and sales prices.

## Project Steps

## 1. Setup

Rename Home_Sales_starter_code.ipynb to Home_Sales.ipynb.

Import necessary PySpark SQL functions.

## 2. Load Data

Read the home_sales_revised.csv file from the AWS S3 bucket into a PySpark DataFrame.

Create a temporary SQL table called home_sales.

## 3. Data Analysis

Execute SparkSQL queries to answer the following:

Average price of four-bedroom homes sold per year (rounded to two decimal places).

Average price of homes with three bedrooms and three bathrooms per year built (rounded to two decimal places).

Average price of homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet per year built (rounded to two decimal places).

Average home price per view rating for homes with an average price ≥ $350,000, and measure query runtime.

## 4. Performance Optimization

Cache the home_sales table and verify caching.

Run the last query on cached data and compare runtime with uncached execution.

Partition the dataset by date_built and save it in Parquet format.

Create a temporary table from the Parquet data and execute the last query again, measuring runtime.

Uncache home_sales table and verify it is uncached.

## 5. Final Steps

Download the completed Home_Sales.ipynb file.

Upload the file to the Home_Sales GitHub repository.

Running the Project

## To run this project:

Install PySpark if not already installed:

!pip install findspark
 open your googlecolab

 or
 
Open Jupyter Notebook and run Home_Sales.ipynb.

Follow the steps in the notebook to load data, run queries, optimize performance, and analyze results.
