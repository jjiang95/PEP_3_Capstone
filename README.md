# AMZN Stock Prices: ETL Pipeline

By using semi-structured data of AMZN stock price sources from the daily-updated [Alpha Vantage API](https://www.alphavantage.co), we will create an ETL pipeline to repeatedly extract, transform, and store data to conduct in-depth analyses both descriptive and inferential.

## Technologies

Python, Pandas, SQLite

## Pipeline

1. Request latest JSON data from API
2. Convert JSON to Pandas dataframe
3. Insert only latest + non-duplicate data into database
4. Entire dataset retrieved from database and converted back into dataframe for analysis
5. Graphs and scatterplots generated for analysis of trends/patterns