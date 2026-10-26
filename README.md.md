# Quantitative Financial Market & Portfolio Performance Analytics

**Submitted by:** Abrin Rithish G S 
**Roll No:** 241501009

## Project overview
This FDVA mini project demonstrates quantitative financial market analysis and portfolio performance tracking using Python, Power BI, and Tableau. The supplied dataset contains sample historical trading data and portfolio metrics. It is designed for educational demonstration of financial analytics techniques.

## Files
- `Financial_Analytics_Mini_Project.pdf` — formatted mini-project report.
- `Financial_Analytics_Mini_Project.docx` — editable report source.
- `Financial_Market_Data.csv` — raw sample dataset containing historical stock/asset prices.
- `Cleaned_Financial_Data.csv` — cleaned dataset formatted for visualisation and dashboard tools.
- `financial_portfolio_analysis.py` — reproducible Python cleaning, metric calculation, and chart-generation script.
- `README.md` — project setup and usage guide.

## Requirements
Python 3.10 or newer; packages: pandas, numpy, matplotlib, and seaborn.
Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn
```

## Run the analysis
Place the raw CSV and Python script in the same folder, then run:
```bash
python financial_portfolio_analysis.py
```
The script loads the raw dataset, handles missing market dates, standardises numeric fields, calculates derived metrics (like daily returns and moving averages), exports `Cleaned_Financial_Data.csv`, and saves the generated chart images.

## Power BI
1. Open Power BI Desktop.
2. Select **Get data → Text/CSV** and import `Cleaned_Financial_Data.csv`.
3. Create KPI cards for **Total Portfolio Return**, **Average Daily Volume**, **Sharpe Ratio**, and **Maximum Drawdown**.
4. Add charts for price trends over time, trading volume by sector, moving average crossovers, and asset correlation.
5. Add slicers for **Ticker Symbol**, **Sector/Asset Class**, and a **Date Range**.
6. Check date sorting and currency/percentage formatting before publishing.

## Tableau
1. Open Tableau Desktop/Public and connect to `Cleaned_Financial_Data.csv`.
2. Create worksheets for monthly portfolio returns, sector allocation, volatility trends, asset performance comparison, and volume analysis.
3. Assemble the worksheets into a "Portfolio Performance Dashboard".
4. Add interactive filters for **Ticker Symbol**, **Sector**, and **Year/Quarter**.

## Data dictionary (selected fields)
- `Date`: trading date.
- `Ticker`: unique symbol for the stock or asset.
- `Sector`: market sector classification (e.g., Technology, Finance).
- `Open_Price`, `Close_Price`: opening and closing prices for the session.
- `High`, `Low`: highest and lowest prices during the session.
- `Volume`: number of shares/units traded.
- `Daily_Return_Pct`: percentage change from the previous day's closing price.
- `Moving_Avg_50`: 50-day moving average price.
- `Volatility_Index`: calculated rolling risk/volatility metric.

## Important note
The dashboard pictures in the report are illustrative layout mockups, not screenshots of live Power BI or Tableau reports. The data and results are generated for educational demonstration. Build the dashboards in the respective applications to obtain working interactive filters and tooltips.