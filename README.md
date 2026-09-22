# Layoffs Data Cleaning & Exploratory Data Analysis

A MySQL project focused on cleaning, standardizing, and exploring a layoffs dataset. The project demonstrates practical SQL techniques for preparing data and extracting insights across companies, industries, countries, funding stages, and time periods.

## Project Overview

The project follows a structured data analysis workflow:

**Raw Data → Data Cleaning → Standardization → Missing-Value Handling → Exploratory Data Analysis**

The SQL script uses MySQL to transform the dataset into a cleaner format before performing analytical queries.

## Data Cleaning

The project includes:

- Identifying duplicate records using `ROW_NUMBER()`
- Creating a cleaned working table
- Removing duplicate records
- Trimming and standardizing company names
- Standardizing industry values
- Cleaning country names
- Converting text dates into SQL `DATE` values
- Identifying and handling missing industry values
- Populating missing industry values using matching company records
- Removing records where both total and percentage layoffs are unavailable
- Removing temporary cleaning columns

## Exploratory Data Analysis

The analysis investigates:

- Maximum and minimum percentage of employees laid off
- Companies with the highest total layoffs
- Layoffs by industry
- Layoffs by country
- Layoffs by year
- Layoffs by funding stage
- Layoff trends over time
- Monthly rolling layoff totals
- Companies with the highest layoffs each year
- Top 5 companies by layoffs for each year

## SQL Techniques Used

- `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`
- `JOIN`
- `UPDATE` and `DELETE`
- `CREATE TABLE`
- `ALTER TABLE`
- `TRIM`
- `STR_TO_DATE`
- Aggregate functions such as `SUM()`, `MAX()`, and `MIN()`
- Common Table Expressions (CTEs)
- Window functions
- `ROW_NUMBER()`
- `DENSE_RANK()`
- Rolling totals
- Date and year-based analysis

## Key Analysis

The project analyzes layoffs across different dimensions, including company, industry, country, funding stage, and year. It also uses monthly aggregation and rolling totals to examine how layoffs changed over time.

Window functions are used to rank companies and identify the top 5 companies by total layoffs for each year.

## Technologies

- MySQL
- SQL
- Common Table Expressions (CTEs)
- Window Functions
- Data Cleaning
- Exploratory Data Analysis

## Repository Structure

```text
Exploratory-Data-Analysis/
│
├── layoffs-cleaning-and-eda.sql
└── README.md
