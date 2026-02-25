# Books Scraper & Analysis

This project scrapes book data from [Books to Scrape](https://books.toscrape.com/)  
and performs basic analysis on the collected dataset.

## How It Works

### 1. Scraping
We use **Scrapy** (a Python web scraping framework) inside **JupyterLab** to:
- Visit the website's book listing pages
- Extract:
  - **Title** → Name of the book
  - **Price** → Price in GBP (£)
  - **Availability** → Whether the book is in stock
  - **URL** → Link to the book's detail page
- Follow pagination until a set limit of books is reached
- Save the results into `books.csv`

**In simple terms:**  
The scraper acts like a robot that clicks through the book pages, reads the title, price, and stock info, and writes it all into a spreadsheet.

### 2. Analysis
Once we have `Books.csv`, we use **Pandas** to explore the data.

We calculate:

#### Dataset Shape
- **What it is:** Number of rows (books) and columns (fields) in the dataset.
- **Why it matters:** Tells us how much data we collected.

#### Average Price
- **What it is:** The mean price of all books.
- **Why it matters:** Gives a quick idea of the general price range.

#### Most Expensive Book
- **What it is:** The single book with the highest price.
- **Why it matters:** Shows the top-priced item in the dataset.

#### Cheapest Book
- **What it is:** The single book with the lowest price.
- **Why it matters:** Shows the most affordable book.

#### Top 10 Most Expensive Books
- **What it is:** A list of the 10 priciest books.
- **Why it matters:** Useful for spotting premium or rare books.

#### Availability Counts
- **What it is:** How many books are "In stock" vs. "Out of stock".
- **Why it matters:** Helps understand stock levels.

## Files in This Repository
- `CodeAlpha Web Scraping.ipynb` → Jupyter Notebook to run the scraper and analyse the dataset
- `Books.csv` → Output dataset (generated after scraping)
- `README.md` → Project documentation

---

# Black Friday Sales – Exploratory Data Analysis

## Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on the Black Friday Sales dataset from Kaggle.

The goal is to uncover patterns in customer purchasing behavior and provide data-driven insights that could inform marketing and sales strategies.

## Business Questions

This analysis aims to answer:

Which demographic groups spend the most?

Does gender significantly influence purchasing behavior?

Which age group has the highest average spending?

How do city categories impact purchase amount?

Are there missing data issues affecting analysis?

## Analytical Approach
### Data Exploration

Inspected structure, data types, and summary statistics

Identified categorical vs numerical variables

### Missing Value Analysis

Detected significant missing values in Product_Category_2 & 3

Applied appropriate imputation strategy

### Trend & Pattern Analysis

Distribution of purchase amounts

Spending by gender, age, and city category

Correlation analysis between numerical variables

### Hypothesis Testing

Compared mean spending across demographic groups

Evaluated statistical significance using t-tests

## Key Insights

Certain age groups exhibit significantly higher average spending.

Male customers tend to have slightly higher total purchase amounts.

City category influences purchasing power.

Product categories show strong skewness in popularity.

## Skills Demonstrated

Python (pandas, NumPy)

Data Cleaning & Preprocessing

Data Visualization (matplotlib, seaborn)

Statistical Testing

Business Insight Interpretation

Structured Analytical Workflow

## Visual Outputs

The project generates:

Purchase distribution plots

Demographic spending comparisons

Group-level statistical summaries
