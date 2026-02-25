# CodeAlpha Data Analysis Internship Projects

This repository contains projects completed during the **CodeAlpha Data Analysis Internship**, focused on **data-driven decision making and business intelligence**.

The projects demonstrate hands-on experience in:

- Web Scraping
- Data cleaning and preprocessing  
- Exploratory Data Analysis (EDA)  
- Statistical analysis and hypothesis testing  
- Data visualization  
- Extracting actionable insights from real-world datasets using Python  

---

# Project 1: Books Scraper & Data Analysis

## Overview

This project combines **web scraping and data analysis**.  
Book data was collected from [Books to Scrape](https://books.toscrape.com/) and analyzed to uncover pricing and availability insights.

The workflow follows a complete data pipeline:

> Data Collection → Data Cleaning → Data Analysis → Insight Generation

---

## Tools Used

- Python  
- Scrapy  
- Jupyter Notebook  
- Pandas  
- Matplotlib / Seaborn  

---

## Data Collection (Web Scraping)

Using **Scrapy**, the scraper:

- Navigates through book listing pages  
- Extracts:
  - Title  
  - Price (GBP £)  
  - Availability  
  - Product URL  
- Handles pagination  
- Stores results in `Books.csv`

The scraper automates browsing and compiles structured data into a dataset ready for analysis.

---

## Data Analysis

After collecting the data, the dataset was analyzed using Pandas.

### Key Analyses Performed

- **Dataset Shape** – Number of books collected  
- **Average Price** – Overall price level  
- **Most Expensive Book** – Highest priced item  
- **Cheapest Book** – Lowest priced item  
- **Top 10 Most Expensive Books** – Premium pricing insights  
- **Availability Breakdown** – Stock distribution  

---

## Files

- `CodeAlpha Web Scraping.ipynb` → Scraper and analysis notebook  
- `Books.csv` → Generated dataset  
- `README.md` → Project documentation  

---

# Project 2: Black Friday Sales – Exploratory Data Analysis

## Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the Black Friday Sales dataset from Kaggle.

Dataset Source:  
https://www.kaggle.com/datasets/pranavuikey/black-friday-sales-eda/data

The objective is to analyze customer purchasing behavior and generate business insights to support marketing and sales strategies.

---

## Business Questions

The analysis addresses:

- Which demographic groups spend the most?
- Does gender significantly influence purchasing behavior?
- Which age group has the highest average spending?
- How does city category affect purchase amounts?
- Are there missing data issues that require cleaning?

---

## Analytical Approach

### Data Exploration
- Reviewed dataset structure and data types  
- Generated descriptive statistics  
- Identified categorical and numerical features  

### Missing Value Analysis
- Detected missing values in `Product_Category_2` and `Product_Category_3`  
- Applied appropriate imputation strategy  

### Trend & Pattern Analysis
- Purchase distribution analysis  
- Spending behavior by gender, age, and city category  
- Correlation analysis between numerical variables  

### Hypothesis Testing
- Compared group-level spending differences  
- Conducted statistical testing (t-tests) to validate findings  

---

## Key Insights

- Customers aged 26–35 represent a high-spending demographic segment  
- Male customers show slightly higher average purchase values  
- City category impacts purchasing behavior  
- Product category distribution is highly skewed  

---

## Skills Demonstrated

- Python (Pandas, NumPy)  
- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Data Visualization (Matplotlib, Seaborn)  
- Statistical Testing  
- Business Insight Interpretation  
- Structured Analytical Workflow  

---

# Why This Repository Matters

These projects demonstrate the ability to:

- Collect and clean raw data  
- Perform structured exploratory analysis  
- Apply statistical reasoning  
- Translate data into business insights  
- Present findings clearly and professionally  

This repository reflects practical analytical skills aligned with **Data Analyst and Business Intelligence roles**.

