# RTCGN
📈 Stock Ranking Prediction using RT-GCN
📌 Overview
This project implements Relational Temporal Graph Convolutional Networks (RT-GCN) for predicting stock rankings using financial news sentiment analysis and historical stock prices.

🔍 Key Features
✅ Sentiment Analysis of financial news headlines

✅ Graph-Based Learning with RT-GCN

✅ Pairwise Ranking Loss for stock ranking optimization

✅ Sector-Based Graph Construction

✅ Spearman’s Rank Correlation for evaluation

📂 Dataset
The dataset includes 5 NIFTY 50 stocks:

HDFCBANK.NS (Banking)

RELIANCE.NS (Oil & Gas)

TCS.NS, INFY.NS (IT)

SBIN.NS (Banking)

📊 Stock Price Data
Source: Yahoo Finance

Features: Close, Open, High, Low, Volume

📰 News Sentiment Data
Source: Economic Times, Moneycontrol, Yahoo Finance

Sentiment labels: Positive (1), Neutral (0), Negative (-1)

Model: DistilBERT-based financial sentiment classifier

📜 Contents of This Notebook
1️⃣ Sentiment Analysis
Scrapes financial news from reliable sources

Applies a DistilBERT-based sentiment classifier

Generates a sentiment-labeled dataset

2️⃣ Stock Data Processing
Loads stock prices from Yahoo Finance

Normalizes and aligns daily stock prices

3️⃣ Graph Construction for RT-GCN
Nodes: Stocks

Edges: Sector-based connections (Banking, IT, Oil & Gas)

Node Features: Stock prices (Close, Open, High, Low, Volume) + Sentiment Scores

4️⃣ Training RT-GCN Model
Uses Relational Graph Convolution (R-GCN)

Temporal dependency with T=5 days

Pairwise Ranking Loss for stock ranking

5️⃣ Evaluation & Results
Computes Spearman’s Rank Correlation

Analyzes how well the model ranks stocks

📌 How to Use
Open the Jupyter Notebook (RTGCN.ipynb).

Run the notebook cell by cell to execute sentiment analysis, data processing, graph construction, training, and evaluation.

📊 Results & Observations
Sentiment analysis helped improve stock ranking accuracy.

Graph-based learning captured sector-wise stock interactions.

The RT-GCN model successfully predicted stock rankings.

📌 Future Improvements
🔹 Expand to more NIFTY stocks

🔹 Incorporate real-time sentiment updates

🔹 Experiment with different graph structures
