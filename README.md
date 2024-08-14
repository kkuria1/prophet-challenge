MercadoLibre Search Traffic & Stock Price Analysis

Overview

This project aims to analyze the relationship between Google search traffic for MercadoLibre and its stock price movements, especially around significant financial events like the release of quarterly financial results. The analysis includes identifying time-based trends, correlating search data with stock price data, and forecasting future search trends using the Prophet time-series model.

Project Structure

notebooks/: Jupyter notebooks containing the analysis steps and visualizations.
data/: Directory containing the datasets used in the analysis.
output/: Directory to save output files such as plots and model forecasts.
README.md: Project overview and instructions (this file).
Data Sources

The analysis uses two primary datasets:

Google Hourly Search Trends Data: Contains hourly search traffic data for MercadoLibre.
Stock Price Data: Includes historical stock price data for MercadoLibre, including opening, closing, high, and low prices.
Analysis Steps

1. Find Unusual Patterns in Google Search Traffic
Objective: Identify any unusual patterns in search traffic during May 2020, the month when MercadoLibre released its quarterly financial results.
Methods: Slicing the data for May 2020, calculating total search traffic, and comparing it with the median monthly traffic across all months.
2. Mine the Search Traffic Data for Seasonality
Objective: Determine if there are predictable seasonal patterns in the search traffic.
Methods: Grouping data by hour, day, and week to identify time-based trends.
3. Relate Search Traffic to Stock Price Patterns
Objective: Investigate the relationship between search traffic and stock price movements.
Methods: Correlating lagged search traffic with stock volatility and returns, and analyzing trends for the first half of 2020.
4. Create a Time Series Model with Prophet
Objective: Forecast future search traffic trends using the Prophet model.
Methods: Setting up the Google search data for the Prophet model, fitting the model, and plotting the forecasted trends.
Requirements

To run the analysis, you'll need the following Python libraries:

pandas
matplotlib
prophet (formerly fbprophet)
numpy
You can install the required libraries using:

bash
Copy code
pip install pandas matplotlib prophet numpy
Usage

Load the Data: Ensure the datasets are placed in the data/ directory.
Run the Notebooks: Open and execute the notebooks in the notebooks/ directory to perform the analysis.
Review the Outputs: Visualize the results and predictions in the output/ directory or directly within the notebooks.
Results

The analysis provides insights into whether significant financial events influence search traffic and whether this traffic can be used to predict stock price movements. Additionally, the time-series forecasting model offers a glimpse into future trends in search traffic.

Conclusion

This project demonstrates the potential to leverage Google search traffic as a proxy for public interest in MercadoLibre and its possible impact on stock price movements. It also highlights the value of time-series forecasting in predicting future trends.

