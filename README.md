# Books Scraper & Analysis

This project scrapes book data from [Books to Scrape](https://books.toscrape.com/)  
and performs basic analysis on the collected dataset.

---

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

---

### 2. Analysis
Once we have `books.csv`, we use **Pandas** to explore the data.

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

---

## Files in This Repository
- `CodeAlpha Web Scraping.ipynb` → Jupyter Notebook to run the scraper and analyse the dataset
- `Books.csv` → Output dataset (generated after scraping)
- `README.md` → Project documentation
