# 📊 News Sentiment & Stock Market Analysis  
### 🚀 Nova Financial Solutions – Financial Intelligence Project

---

## 🧠 Overview

Financial markets are driven by both numbers and narratives. This project explores how **financial news sentiment** relates to **stock price movements**, and whether market emotions extracted from headlines can help explain or predict returns.

At Nova Financial Solutions, the goal is to build smarter forecasting systems by combining:
- 📰 Financial news (text data)
- 📈 Stock market prices (time-series data)
- 📊 Technical indicators (market behavior signals)
- 🔗 Statistical correlation analysis (relationship testing)

This project builds a complete pipeline from raw data → sentiment → indicators → insights.

---

## 🎯 Business Objective

Nova Financial Solutions aims to improve predictive analytics by integrating alternative data sources into investment decision-making.

This project answers a key question:

> Can financial news sentiment be used as a reliable signal for stock market prediction?

To explore this, we:
- Convert news headlines into sentiment scores
- Align sentiment with stock trading data
- Analyze technical indicators
- Measure statistical relationships between sentiment and returns

---

## 📁 Project Structure
news-sentiment-analysis/
│
├── data/ # Raw datasets (news + stock data)
├── notebooks/ # Jupyter analysis notebooks
├── src/ # Reusable source code
├── scripts/ # Helper scripts
├── tests/ # Unit tests
│
├── .github/
│ └── workflows/ # CI/CD pipeline (GitHub Actions)
│
├── requirements.txt # Dependencies
└── README.md # Project documentation


---

## ⚙️ Tech Stack

- 🐍 Python (3.10+)
- 🧮 Pandas, NumPy (data processing)
- 📊 Matplotlib, Seaborn (visualization)
- 🧠 NLTK (VADER sentiment analysis)
- 📉 TA-Lib (technical indicators)
- 📐 SciPy (statistical analysis)
- 📓 Jupyter Notebook (analysis workflow)
- ⚙️ GitHub Actions (CI/CD pipeline)

---

## 🔄 Workflow

The project follows a structured 3-stage pipeline:

---

## 1️⃣ Exploratory Data Analysis (EDA)

We explored financial news to understand its structure and behavior.

Key insights:
- News is highly **event-driven** (earnings, market events)
- A small number of publishers dominate content
- News is concentrated during trading hours
- Headlines contain recurring financial themes

---

## 2️⃣ Technical Indicator Analysis

Stock prices were analyzed using standard trading indicators:

- 📈 SMA (Simple Moving Average)
- 📈 EMA (Exponential Moving Average)
- ⚡ RSI (Relative Strength Index)
- 🔁 MACD (Momentum Indicator)

Key insights:
- EMA reacts faster to price changes than SMA
- RSI identifies overbought/oversold conditions
- MACD highlights momentum shifts and trend reversals

---

## 3️⃣ Sentiment & Correlation Analysis

We converted news headlines into sentiment scores and compared them with stock returns.

Process:
- Sentiment scoring using VADER
- Daily aggregation of sentiment values
- Computation of stock returns
- Pearson correlation analysis

Key insight:
> Sentiment alone shows weak correlation with daily stock returns.

---

## 📊 Key Insights

- Financial news is highly **event-driven**
- News sentiment is mostly **neutral**
- Technical indicators show stronger structure than sentiment
- Sentiment has **weak predictive power alone**
- Market behavior is influenced by multiple external factors

---

## 📉 Key Finding

> There is a weak and inconsistent linear relationship between financial news sentiment and short-term stock returns.

This means sentiment alone is not enough to predict market movement reliably.

---

## 💡 Investment Strategy Insights

A better approach is combining signals:

✔ Use RSI & MACD for timing trades  
✔ Use sentiment as confirmation  
✔ Focus on high-impact news events  
✔ Combine technical + sentiment signals for stronger decisions  

---

## ⚠️ Limitations

- Sentiment model (VADER) struggles with financial nuance
- Market reactions may be delayed (lag effect not fully captured)
- Averaging sentiment can dilute major news impact
- Only one stock dataset analyzed
- External macroeconomic factors not included

---

## 🚀 Future Improvements

- 🔥 Use FinBERT (financial NLP model)
- ⏳ Add lag-based sentiment analysis (1–3 days)
- 📊 Expand to multiple stocks & sectors
- 🤖 Apply machine learning models for prediction
- 🌍 Include macroeconomic indicators

---

## 🧪 How to Run

```bash
# Clone repository
git clone https://github.com/your-username/news-sentiment-analysis.git
cd news-sentiment-analysis

# Create virtual environment
python -m venv .venv
source .venv/bin/activate   # Mac/Linux
.venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Launch notebooks
jupyter notebook

🔄 CI/CD Pipeline

Automated GitHub Actions workflow ensures code quality and testing.

📁 Location:

`.github/workflows/unittests.yml`
