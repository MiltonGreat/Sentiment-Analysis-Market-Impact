# Sentiment-Analysis-Market-Impact

![screenshot-localhost_8888-2025 03 30-19_00_59](https://github.com/user-attachments/assets/ad660475-d709-4982-9cc6-c873c9813cd0)

## Overview


This project aims to explore how financial news sentiment affects stock prices using Natural Language Processing (NLP) techniques. The goal is to analyze financial news articles, classify their sentiment (bullish, bearish, neutral), and examine how these sentiments may influence stock market movements. By leveraging a combination of VADER and TextBlob sentiment analyzers, along with a domain-specific financial lexicon, we can gain insights into the relationship between financial news and market behavior.

### Key Features

- Sentiment Analysis: Sentiment of financial news articles is classified as bullish, bearish, or neutral using enhanced VADER and TextBlob models.

- Financial Lexicon Enhancement: A financial-specific lexicon is incorporated into VADER to improve its handling of financial terms like "rally", "slump", "surge", etc.

- Batch Processing: Efficient processing of large datasets in batches to ensure scalability.

- Market Impact Visualization: Sentiment distribution of financial news articles is visualized to better understand the sentiment landscape.

- Stock Market Price Prediction: Potential extension to predict stock price movement based on sentiment (can be added later for a more complete model).

### Project Workflow

1. Load Data

Ensure that your financial news data is in CSV format with columns like date, Headlines, and Description. You can use the cleaned_news_data.csv file for testing.

2. Sentiment Analysis

This project uses an enhanced VADER sentiment analyzer that incorporates a custom financial lexicon. The following steps are performed:

- Each article’s headline and description are concatenated to form the full text.
- Sentiment scores are calculated using VADER and TextBlob.
- A weighted average of the VADER and TextBlob scores is used to classify the sentiment as bullish, bearish, or neutral.

3. Batch Processing

To process large datasets efficiently, sentiment analysis is performed in batches. This helps to track progress and save intermediate results, minimizing the risk of losing data if the process is interrupted.

4. Visualize Sentiment Distribution

The sentiment distribution of the entire dataset is plotted as a bar chart. The sentiment labels (bullish, bearish, neutral) are visualized for easy analysis.

### Future Improvements

1. Stock Price Prediction: Integrate sentiment with stock market data to build predictive models that forecast price movements based on sentiment.

2. Model Optimization: Experiment with other sentiment analysis models like FinBERT for improved accuracy.

3. Extended Analysis: Analyze the correlation between sentiment and market movements to quantify the impact of financial news.

### Source

[Financial News Headlines Data from Kaggle](https://www.kaggle.com/datasets/notlucasp/financial-news-headlines#%20Sentiment%20Analysis%20in%20Finance)
