# Week1-Financial-News-Analytics

## 📌 Project Overview
This repository analyzes **financial news, stock price data, and their correlations**, integrating:
- Exploratory Data Analysis (EDA)
- Quantitative stock indicators using **TA-Lib** and **PyNance**
- Sentiment analysis on financial news
- Correlation between news sentiment and stock movement

---

## 📊 Key Insights from Week 1 (News Dataset)
- The dataset focuses heavily on **stocks, earnings, analyst ratings, and price targets**.
- From **2012 to 2019**, news volume remained steady.
- Starting **late 2019**, article count increased sharply.
- **2020** had the biggest spike, mainly driven by:
  - **Lisa Levin**
  - **Benzinga Newsdesk**

These contributors published a high number of market-moving articles that influenced overall trends.

---

# 🧩 Task 2 — Quantitative Analysis Using PyNance & TA-Lib

## 🎯 Objectives
- Load and prepare stock price data (OHLCV)
- Apply technical indicators using **TA-Lib**
- Compute financial metrics with **PyNance**
- Visualize stock trends and indicators
- Follow Git workflow (branches, commits, PRs)

---

## ✅ Minimum Essential To Do (Task 2)
- Merge necessary **task-1** branches → `main` using Pull Request (PR)
- Create a new branch: **`task-2`**
- Commit progress with **clear, descriptive** commit messages
- Prepare stock data
- Calculate basic indicators (SMA, EMA, RSI, MACD, etc.)
- Visualize the results (price charts, indicator overlays)

---

## 🛠️ Steps for Task 2

### 1. Prepare Your Data
- Load stock data into pandas  
- Ensure columns: **Open, High, Low, Close, Volume**
- Convert date columns to datetime

### 2. Calculate Technical Indicators (TA-Lib)
Examples:
- **SMA / EMA**
- **RSI – Relative Strength Index**
- **MACD – Moving Average Convergence Divergence**
- **Bollinger Bands**
- **ATR – Average True Range**

### 3. Use PyNance for Financial Metrics
- Daily Returns  
- Rolling Volatility  
- Sharpe Ratio  
- Drawdowns  

### 4. Visualizations
- Candlestick charts  
- Price vs SMA/EMA  
- RSI plots  
- MACD plots  

---

# 🧩 Task 3 — Correlation Between News and Stock Movement

## 🎯 Objectives
- Align dates between news and stock data
- Perform sentiment analysis on headlines
- Calculate daily stock returns
- Compute correlation between sentiment and stock movement

---

## ✅ Minimum Essential To Do (Task 3)
- Merge **task-2** → `main` via PR  
- Create new branch: **`task-3`**
- Commit work with descriptive messages
- Prepare news + stock data
- Normalize dates
- Perform sentiment scoring
- Calculate returns and correlation

---

## 🛠️ Steps for Task 3

### 1. Normalize Dates
- Standardize timestamps  
- Align news to stock trading days  
- Handle weekends + missing days  

### 2. Sentiment Analysis
Tools:
- **NLTK**
- **TextBlob**
- (Optional) VaderSentiment / HuggingFace transformers  

Outputs:
- Polarity scores  
- Pos/Neg/Neutral labels  
- Daily aggregated sentiment  

### 3. Stock Movement Calculations
- Calculate **daily % returns** from closing prices  
- Clean missing values  

### 4. Correlation Analysis
- Merge daily sentiment with daily returns  
- Compute **Pearson correlation coefficient**
- Visualize:
  - Sentiment vs Returns over time  
  - Scatter plots  
  - Heatmaps  

---

# 📁 Folder Structure

Week1-Financial-News-Analytics/
│
├── Data/ # Raw + cleaned datasets
├── notebooks/ # Jupyter notebooks for Tasks 1–3
├── scripts/ # Python scripts for indicators, sentiment, correlation
├── visualizations/ # Generated plots and charts
├── README.md # Project documentation
└── requirements.txt # Python packages required

yaml
Copy code

---

# ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Bezawit-cloud/Week1-Financial-News-Analytics.git
cd Week1-Financial-News-Analytics
2. Create Virtual Environment
bash
Copy code
python -m venv .venv
Activate:

Windows

bash
Copy code
.venv\Scripts\activate
Mac/Linux

bash
Copy code
source .venv/bin/activate
3. Install Dependencies
bash
Copy code
pip install -r requirements.txt
🚀 Usage
Open Jupyter Notebook
bash
Copy code
jupyter notebook
Run analysis in notebooks/

Use scripts/ for reusable code

Check visualizations/ for generated charts

📌 KPIs for Evaluation
Task 2 KPIs
Proactive learning + references

Accuracy of technical indicators

Completeness of stock analysis

Quality of visualizations

Task 3 KPIs
Correct sentiment analysis implementation

Proper date alignment

Strength + interpretation of correlation

Data preparation quality
