# Mango Market Price Analysis & Agricultural Market Intelligence

## Project Overview

This project analyzes mango market data from Maharashtra, India, using Python, web scraping, exploratory data analysis (EDA), and Microsoft Power BI.

The objective is to explore market-level price differences, monthly price trends, mango arrivals, variety-wise pricing, and sales quantity patterns. The project combines data collection and preparation with statistical exploration and interactive dashboard visualization.

## Business Objectives

- Analyze mango prices across agricultural markets.
- Compare minimum, maximum, and modal prices.
- Examine monthly price and arrival patterns.
- Investigate the relationship between market arrivals and modal prices.
- Identify markets with higher average modal prices.
- Compare price spreads across markets.
- Analyze quantities by district and mango variety.
- Present key indicators through a Power BI dashboard.

## Tools and Technologies

| Technology | Purpose |
|---|---|
| Python | Data collection and analysis |
| Pandas | Data cleaning and aggregation |
| Requests | Retrieving web pages |
| Beautiful Soup | HTML parsing |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Analytical workflow |
| Microsoft Excel | Dataset inspection |
| Microsoft Power BI | Interactive dashboards |

## Dataset

The supplied Excel workbook contains 1,798 records and 13 columns, with reported dates from January 15 to October 18, 2025.

The dataset represents:
- 13 districts
- 23 market names
- 3 mango variety categories

The main fields include district, market, variety, arrivals, minimum price, maximum price, modal price, and reported date.

The workbook also includes derived or additional fields for month, price spread, sales quantity, sales value, and selling price. The provenance and calculations of sales-related fields require validation before interpreting them as actual financial results.

## Project Workflow

### 1. Web Scraping
- Retrieve agricultural market information from AGMARKNET.
- Extract HTML tables using pandas.
- Use Beautiful Soup as a fallback for table extraction.
- Standardize column names and convert data types.

### 2. Data Cleaning
- Convert numeric fields.
- Parse reporting dates.
- Calculate price spread.
- Review missing values, duplicates, and inconsistent categories.
- Validate derived fields.

### 3. Exploratory Data Analysis
- Monthly average modal price analysis.
- Market-wise price comparisons.
- Arrivals versus modal price analysis.
- Minimum, maximum, and modal price distributions.
- Market-wise price spread analysis.
- Variety-wise price comparisons.
- District-wise quantity analysis.

### 4. Power BI Dashboard
The report contains:
- KPI cards for revenue, quantity, average selling price, and price volatility.
- Arrival and sales quantity visuals.
- District-wise quantity comparisons.
- Variety-wise selling-price comparisons.
- District and variety slicers.

#### Dashboard - 
![Power BI Dashboard](https://github.com/VishwasJadhav/Mango-Market-Price-Analysis/blob/main/Power%20BI%20Dashboard/Dashboard%20Screenshot.png)
## Preliminary Observations

- The supplied workbook contains 1,798 records across 23 markets.
- Hapus (Alphaso) has a higher average modal price than the other variety categories in the supplied data.
- Mumbai- Fruit Market has the highest average modal price among the markets in the dataset.
- Mumbai- Fruit Market also has the highest average price spread in the supplied records.

## Limitations

- The dataset covers a limited reporting period.
- Monthly record counts are uneven.
- Price differences may reflect variety, quality, market, and reporting conditions.
- Sales and revenue measures require validation.
- The scraping workflow may need maintenance if the source website changes.
- The analysis is descriptive and does not establish causation.

## Future Improvements

- Automate scheduled data collection.
- Improve duplicate detection and data validation.
- Add correlation and regression analysis.
- Compare equivalent varieties across markets and dates.
- Develop a statistically rigorous price-volatility measure.
- Validate financial KPIs and document derived fields.
- Improve dashboard usability and reproducibility.

## Data Source

AGMARKNET: https://agmarknet.gov.in/
