# ACC102 Data Product: Real Estate Investment Analysis

## 1. Problem & User
This project analyzes the key drivers of real estate prices to assist a **Real Estate Investment Trust (REIT)** in optimizing their property acquisition strategy. The goal is to understand how location, local income, and property features impact valuations.

## 2. Data
* **Source:** California Housing Dataset (fetched directly from Ageron's Hands-on ML GitHub repository via URL).
* **Access Date:** April 2026.
* **Key Fields:** `median_house_value`, `median_income`, `ocean_proximity`, `longitude`, `latitude`.

## 3. Methods
* **Data Loading:** Used `pandas` to read CSV directly via URL for seamless reproducibility.
* **Data Cleaning:** Imputed missing values in `total_bedrooms` using the median to maintain data integrity against outliers. Created a new feature (`rooms_per_household`).
* **Analysis & Visualization:** Utilized `matplotlib` and `seaborn` to generate five analytical charts (Histograms, Scatter Maps, Bar Charts, Heatmaps) to uncover correlations.

## 4. Key Findings
* **Income Correlation:** Median income is the strongest predictor of house value (Correlation coefficient: 0.69).
* **Geographical Impact:** Prices are highest near the coastlines (Bay Area and Los Angeles clusters).
* **Category Premium:** Properties categorized as "Near Bay" or "Near Ocean" hold significantly higher average valuations than "Inland" properties.

## 5. How to run
1. Ensure you have Python installed along with `pandas`, `numpy`, `matplotlib`, and `seaborn`.
2. Open `notebook.ipynb` in Jupyter Notebook or JupyterLab.
3. Run all cells sequentially. No local CSV downloads are required as the script fetches data directly from the web.

## 6. Product link / Demo
* **Demo Video Link:** [Insert your Mediasite/YouTube link here]
* **Repository Link:** [Insert this GitHub Repo URL here]

## 7. Limitations & next steps
* **Limitation:** The dataset represents a historical snapshot and does not account for current macroeconomic changes like recent interest rate hikes.
* **Next Step:** Integrate a predictive machine learning model (e.g., Random Forest) to forecast undervalued properties.
