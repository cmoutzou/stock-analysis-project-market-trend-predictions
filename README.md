# stock-analysis-project-market-trend-predictions
A Python project for analyzing stock market trends using historical data. Includes data processing, visualization, and basic predictive analytics.
## Description
The Financial Analysis and Prediction Toolkit is a Python-based project designed to fetch financial data, analyze it, and make predictions using various statistical and machine learning models. The toolkit integrates with multiple data sources and APIs, including Yahoo Finance and Alpha Vantage, and uses advanced techniques such as ARIMA, LSTM, and Prophet for time series forecasting.

Features
Data Fetching: Retrieve historical and real-time stock data from Yahoo Finance and Alpha Vantage.
Technical Analysis: Compute various financial indicators such as Moving Averages, RSI, MACD, Bollinger Bands, and ATR.
Predictive Modeling: Apply ARIMA, LSTM, and Prophet models to forecast future stock prices.
Sentiment Analysis: Analyze the sentiment of news headlines related to stocks.
Macroeconomic Analysis: Integrate and analyze macroeconomic indicators from the Federal Reserve Economic Data (FRED) API.
Visualization: Generate interactive charts to visualize historical data, predictions, and technical indicators.
Installation
To set up the project, you'll need to install the required Python libraries. You can use pip to install these dependencies. Ensure you have Python 3.7 or later installed.

Clone the Repository

bash
Copy code
git clone https://github.com/cmoutzou/financial-analysis-toolkit.git
cd financial-analysis-toolkit
Install Dependencies

bash
Copy code
pip install -r requirements.txt
You can also install the required packages individually if requirements.txt is not available:

bash
Copy code
pip install requests yfinance pandas numpy fredapi matplotlib textblob beautifulsoup4 seaborn plotly statsmodels tensorflow prophet scikit-learn
Configuration
API Keys

Alpha Vantage: You need to obtain an API key from Alpha Vantage. Replace "your_alpha_vantage_api_key" in the code with your actual API key.
FRED API Key

Obtain an API key from the Federal Reserve Economic Data (FRED) website and replace '38a85b8262a0044479cc6200b3c2c99f' with your actual API key in the code.
Usage
Running the Analysis

Run the script to perform the analysis:

bash
Copy code
python main.py
This will process the specified stock symbols, fetch the data, compute indicators, perform sentiment analysis, and generate predictions and charts.

Modifying Symbols

You can adjust the list of stock symbols in the symbols variable within the script to analyze different stocks:

python
Copy code
symbols = ["AAPL", "NVDA", "TSLA"]
Adjusting Parameters

Modify the period and interval parameters to change the timeframe of the data used for analysis:

python
Copy code
process_symbol(symbol, '1y', '1d')
period can be '1d', '1mo', '6mo', '1y', '5y', '10y', etc.
interval can be '1m', '5m', '15m', '30m', '1h', '1d', etc.
Key Components
Data Fetching Functions: Retrieve stock data from Yahoo Finance and Alpha Vantage.
Indicator Calculation: Functions to calculate various technical indicators.
Prediction Models: ARIMA, LSTM, and Prophet models for forecasting stock prices.
Visualization: Plotly for interactive charting and visualization of data and predictions.
Sentiment Analysis: Analyze the sentiment of news headlines using TextBlob.
Example Output
The script generates interactive plots for stock price predictions, including:

Historical and predicted prices from ARIMA and LSTM models.
Technical indicators like Moving Averages, Bollinger Bands, and MACD.
News sentiment analysis results.
Macroeconomic indicators and their impact.
Contribution
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.
