📊 Stock Trend Prediction Using Machine Learning
Capstone Project Portfolio
Tech Stack: Python, Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn, Plotly, TextBlob, VADER, Yahoo Finance API

🔍 Project Overview
The objective of this capstone project was to develop an advanced machine learning system to predict stock price movements by integrating both numerical and textual data. The model utilizes historical stock prices and sentiment analysis from financial news sources to improve the accuracy of stock trend forecasting.

📌 Problem Statement
Traditional methods of stock prediction often fall short in capturing the real-time sentiments and complex market behaviors. Our project aimed to enhance stock trend prediction by combining historical price data with sentiment scores derived from news headlines and articles, thereby helping investors make informed decisions.

🔧 Approach and Methodology
1. Data Collection
Stock Price Data: Fetched Microsoft (MSFT) stock data from 2000 to 2023 using the yfinance API.

News Data: Collected and cleaned financial news articles containing titles, publication dates, and sources.

2. Data Cleaning
Removed duplicates and null values from news data.

Extracted relevant fields (title, source, publication date) and converted to a structured format.

Used eval() to extract nested JSON elements for source and author URLs.

3. Sentiment Analysis
Applied VADER to compute compound sentiment scores (ranging from -1 to 1).

Used TextBlob to derive subjectivity and polarity scores.

Created word clouds to visualize dominant sources and authors.

Merged daily news into a single text body to compute daily sentiment metrics.

4. Model Building
Used Naive Bayes Classifier from Scikit-learn as the base model.

Trained on historical sentiment and stock data (Training: 2005–2021, Testing: 2022–2023).

Evaluated with accuracy score, confusion matrix, and classification report.

📈 Key Results
Calculated the proportion of positive vs. negative sentiment across the dataset.

Achieved a large proportion (~90%) of positive sentiment from news headlines.

Demonstrated the potential of sentiment-driven machine learning in predicting stock trends.

📌 Visualizations and Insights
Line plots of historical MSFT stock trends using Plotly.

Word clouds of frequent news sources and authors.

Pie chart showing sentiment distribution (positive vs. negative).

✅ Key Learnings
Integration of textual data with numeric stock data enhances prediction quality.

Sentiment analysis adds a human perspective to machine predictions.

Preprocessing and data cleaning are vital for model accuracy.

Challenges in aligning dates between news and stock data were successfully handled.
