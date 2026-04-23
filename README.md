# ACC102 Data Product: Real Estate Investment Analysis - California Housing Market

## 1. Problem & User
The objective of this data product is to identify the fundamental drivers of real estate prices in the California housing market. The intended user is a **Real Estate Investment Trust (REIT) investment team** looking to optimize their property acquisition strategy by understanding how location, local demographics, and property features impact financial valuations.

## 2. Data
* **Source:** California Housing Dataset. To ensure seamless reproducibility and avoid local file path errors, the data is fetched directly via a stable URL from the *Hands-on Machine Learning* public repository.
* **Access Date:** April 2026
* **Key Fields Used:** `median_house_value` (target variable), `median_income`, `ocean_proximity`, `longitude`, `latitude`, `total_rooms`, and `total_bedrooms`.

## 3. Methods
This project features a coherent Python-based analytical workflow:
* **Data Acquisition:** Used `pandas` to read the CSV directly from the web URL.
* **Data Cleaning & Preparation:** Identified missing values in the `total_bedrooms` column and imputed them using the median to maintain robustness against outliers. 
* **Feature Engineering:** Created a new metric, `rooms_per_household`, to provide a standardized measure of property size.
* **Analysis & Visualization:** Utilized `matplotlib` and `seaborn` to generate five analytical charts, including a geographical scatter map (combining coordinates, population, and price), a correlation heatmap, and distribution plots to uncover business insights.

## 4. Key Findings
1. **Income is the Strongest Predictor:** The correlation heatmap mathematically proves that local median income has the strongest positive correlation (0.69) with housing values.
2. **The "Location Premium":** Properties categorized as "Island" or "Near Bay" command significantly higher average valuations than "Inland" properties.
3. **Coastal Value Clusters:** The geographical scatter plot clearly visualizes that the highest value properties are densely clustered along the coastlines (specifically the Los Angeles and Bay Area regions), confirming that geographical proximity to the ocean drives asset value.

## 5. How to Run
This project is designed to be highly reproducible. No local data download is required.
1. Clone or download this repository.
2. Ensure you have a Python environment installed with the following libraries: `pandas`, `numpy`, `matplotlib`, and `seaborn`.
3. Open `notebook.ipynb` using Jupyter Notebook or JupyterLab.
4. Click **"Run All"** cells. The notebook will automatically fetch the data from the web and generate all five visualizations.

## 6. Product Link / Demo
* **Demo Video Link:** [请在这里替换成你的 Mediasite 视频链接]
* **GitHub Repository Link:** [请在这里替换成你的 GitHub 仓库链接]

## 7. Limitations & Next Steps
* **Limitations:** The current dataset represents a historical snapshot and lacks temporal dynamics. Real estate markets are highly cyclical, and this static data does not account for recent macroeconomic factors such as inflation, mortgage interest rate hikes, or post-pandemic migration trends.
* **Next Steps:** To improve this product for the REIT investment team, the next step would be to integrate a predictive machine learning model (such as a Random Forest Regressor) to automatically flag undervalued properties in high-income neighborhoods.
