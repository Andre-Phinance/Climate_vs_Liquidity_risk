# Financial and Climate Analysis Project

## Overview
This project explores the relationship between the financial ratios of major Canadian banks and climate variables over time. The banks analyzed are:
- Royal Bank of Canada (RY.TO)
- Toronto-Dominion Bank (TD.TO)
- Bank of Nova Scotia (BNS.TO)

The climate variables studied include:
- Mean Sea Level (Sea_Lvl_M)
- Cooling Degree Days Mean (CDD_M)
- Maximum 5-Day Precipitation (Rx5Day_M)
- 10th Percentile Temperature (T10_M)
- 90th Percentile Temperature (T90_M)
- 90th Percentile Wind Speed (WP90_M)

## Methodology
- **Data Collection**: Financial data was obtained via [Ycharts](https://ycharts.com/stocks), while climate data was sourced from the [Actuaries Climate Index](https://actuariesclimateindex.org/home/), all stored in .xlsx files.
- **Data Processing**: Missing values in financial ratios were filled using a moving average based on periods t-1 and t+1. Monthly climate data was aggregated into quarterly averages.
- **Analysis**: Linear and log-linear regression models were used to assess the impact of climate variables on financial ratios such as the **Cash Ratio**, **Quick Ratio**, and **Current Ratio**.

## Tools and Libraries
The following tools and libraries were used in this project:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `plotly`
- `statsmodels`
- `scipy`
- `sklearn`
- `yfinance`

## Visualizations
The project includes several visualizations:
- Time series plots showing trends in financial ratios and climate variables.
- Fitted log-linear regression curves to illustrate modeled relationships.

## Results
The results include summaries of the regression models with:
- Coefficients
- P-values
- R² (coefficient of determination)
- Mean Squared Error (MSE)

These metrics help evaluate the relationship between climate variables and financial ratios.

## How to Run the Code
1. Ensure all the listed libraries are installed (`pip install -r requirements.txt` if a `requirements.txt` file is provided).
2. Place the data files (Excel files for climate and financial data) in the local environment to properly execute the code.
3. Run the Jupyter notebook or Python script to start the analysis.

## Disclaimer
This project is a study based on historical data. The results should be interpreted with caution and do not constitute a prediction of future performance.
