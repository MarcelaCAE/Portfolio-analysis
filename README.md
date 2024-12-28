# Financial Data Analysis Project

## Objective of the Project
The primary objective of this project is to analyze asset price data, conduct Exploratory Data Analysis (EDA), calculate portfolio returns, and perform portfolio analysis. The goal is to gain insights into asset price behavior over time and make informed decisions regarding portfolio construction and management. 

## Dataset Overview:
The project uses three key datasets:

### 1. **asset_information_data.csv**
   This dataset contains information about the assets in the portfolio, including their **Name** and **Family** (the asset class).

   **Columns:**
   - **Name**: The name of the asset (e.g., `Asset1`, `Asset2`, `Asset3`, etc.)
   - **Family**: The asset class/category (e.g., `Fixed Income`, `Equity`, `Alternative`).

### 2. **asset_price_data.csv**
   This dataset contains historical asset prices over time. The asset prices are recorded with a date column, and each asset (Asset1, Asset2, Asset3, Asset4, Asset5) has its own column containing the price data for that asset.

   **Columns:**
   - **Date**: The date of the data point.
   - **Asset1**: The price data for Asset1 on the corresponding date.
   - **Asset2**: The price data for Asset2 on the corresponding date.
   - **Asset3**: The price data for Asset3 on the corresponding date.
   - **Asset4**: The price data for Asset4 on the corresponding date.
   - **Asset5**: The price data for Asset5 on the corresponding date.

### 3. **portfolio_weights.csv**
   This dataset contains the asset allocation (weights) in the portfolio over time. Each row corresponds to a specific date, and the portfolio's weights for each asset (Asset1, Asset2, Asset3, Asset4, Asset5) are recorded on that date.

   **Columns:**
   - **Date**: The date of the asset allocation data.
   - **Asset1**: The weight of Asset1 in the portfolio on the corresponding date.
   - **Asset2**: The weight of Asset2 in the portfolio on the corresponding date.
   - **Asset3**: The weight of Asset3 in the portfolio on the corresponding date.
   - **Asset4**: The weight of Asset4 in the portfolio on the corresponding date.
   - **Asset5**: The weight of Asset5 in the portfolio on the corresponding date.


### Methodology


### 1. **Data Extraction and Initial Setup**
   - Data was extracted from a CSV file (`asset_price_data (1).csv`) and loaded into a Pandas DataFrame.
   - Column names were standardized by converting them to lowercase and replacing spaces with underscores for consistency.
   - A copy of the dataset (`pricing_data`) was created for further analysis to prevent altering the original data.

### 2. **Data Cleaning**
   - **Datetime Formatting:** The 'date' column was converted into a proper datetime format to facilitate time-based analysis.
   - **Null Values and Duplicates:** The dataset was inspected for missing values and duplicate rows. Checked for empty spaces in the dataset to ensure data integrity.
   
### 3. **Exploratory Data Analysis (EDA)**
   - **Descriptive Statistics:** A statistical summary of the numerical columns was computed to provide an overview of the dataset (including mean, standard deviation, min, max, etc.).
   - **Distribution Plots:** Histograms for each numerical column were plotted to analyze the distribution of asset prices.
   - **Correlation Analysis:** Pearson and Spearman correlation matrices were calculated to explore relationships between different assets. The correlation matrices were visualized using heatmaps for clarity.

### 4. **Calculating Returns**
   - **Daily Returns:** The daily returns were computed for each asset based on the percentage change in asset prices.
   - **Cumulative Returns:** The cumulative returns for each asset were calculated by multiplying the daily returns incrementally over time.
   - **Mean Daily Returns and Volatility:** The mean daily returns and standard deviation (volatility) for each asset were calculated to assess the assets' performance and risk.

### 5. **Portfolio Analysis**
   - **Asset Weights Over Time:** The changes in asset weights over time were visualized using an area chart to provide insights into how portfolio allocation evolved.
   - **Cumulative Returns:** Cumulative returns of the portfolio were calculated to track its overall performance over time.
   - **Annualized Return and Volatility:** These metrics were calculated to assess the risk-adjusted return of the portfolio. Annualized return was computed based on the mean daily return, and annualized volatility was derived from the daily returns' standard deviation.



#### Next Steps:
The next steps would be performed Portfolio Optimization and Risk-Return Analysis.

#### Deliverables
1. Jupyter Notebook: Contains the complete EDA, visualizations, and insights.
2. PowerPoint Presentation: Summarizes the key findings of the project, highlighting the results with clear and impactful visualizations to facilitate communication of the insights.
