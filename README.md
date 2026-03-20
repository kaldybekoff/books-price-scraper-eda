# Books Price Scraper & Exploratory Data Analysis

## Overview
This project demonstrates a simple end-to-end data workflow: web scraping, data cleaning, feature engineering, and exploratory data analysis (EDA).

Using data collected from **books.toscrape.com**, the notebook scrapes book listings, cleans price values, converts them from GBP to USD, groups books into price categories, and explores the overall price distribution of the catalog.

## Goal
The goal of this project is to show a practical data analysis pipeline starting from raw web data and ending with a clean, analysis-ready dataset and interpretable visual insights.

## Data Source
Source website: **http://books.toscrape.com**

The dataset is collected directly by scraping pages **1–50** of the catalogue.

### Collected fields
- `Title`
- `Raw_Price`
- `Availability`

### Engineered fields
- `Price_USD`
- `Price_MinMax`
- `Price_Category`

## Tools & Libraries
- Python
- Jupyter Notebook
- requests
- BeautifulSoup
- pandas
- numpy
- matplotlib

## Workflow
1. Scrape book listings from multiple catalogue pages
2. Extract title, price, and availability
3. Clean raw price strings and convert prices to numeric format
4. Convert GBP prices to USD
5. Create normalized and categorized price features
6. Perform exploratory data analysis with summary statistics and visualizations
7. Identify the cheapest and most expensive books in the dataset

## Key Analysis
The notebook includes:
- price distribution analysis
- boxplot for spread and outliers
- average price by price category
- top most expensive books
- top cheapest books

## Main Insights
- The scraped dataset contains **1,000 books**
- Book prices range roughly from **$12.50 to $74.99**
- The average book price is around **$43.84**
- The median book price is around **$44.98**
- Books are grouped into **Low**, **Medium**, and **High** price categories
- The dataset provides a clear example of how scraped web data can be transformed into a structured dataset for analysis

## Project Structure
```text
.
├── Books Price Scraper & Exploratory Data Analysis.ipynb
├── README.md
