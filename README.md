# acc102-retail-finance-analysis
# Comparative Financial Analysis: Walmart (WMT) vs. Target (TGT)

## 1. Problem & User
The primary analytical problem is to evaluate the financial stability and market performance of retail giants WMT and TGT during market fluctuations (2020-2024). [cite_start]The intended users are entry-level retail investors who need simplified financial insights to make informed decisions[cite: 38].

## 2. Dataset
- [cite_start]**Source**: Yahoo Finance API via `yfinance` library.
- [cite_start]**Access Date**: April 22, 2026[cite: 45].
- **Key Fields**: Adjusted Close Price, Net Income, Total Revenue, and Volatility metrics.

## 3. Methods
This project uses Python to perform:
- **Data Acquisition**: Automated downloading of stock prices and financial statements.
- **Data Cleaning**: Handling missing values and synchronizing time series for comparison.
- [cite_start]**Analysis**: Calculating Net Profit Margins and Annualized Volatility using `pandas`[cite: 37, 129].
- **Visualisation**: Comparative line charts for price trends and bar charts for margins.

## 4. Key Findings
- Walmart (WMT) exhibited lower stock price volatility compared to Target (TGT) over the 4-year period.
- Despite Target's higher volatility, it maintained slightly higher profit margins in specific quarters of 2021.
- Both companies showed strong recovery patterns post-2022.

## 5. How to Run
1. Clone this repository: `git clone https://github.com/yourusername/acc102-retail-finance-analysis.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the `analysis.ipynb` notebook.

## 6. Product Link
- [Link to Python Notebook](./analysis.ipynb)

## 7. Limitations
- The analysis is limited to historical data and does not account for qualitative factors like leadership changes.
- Market sentiment data from social media is not included.
