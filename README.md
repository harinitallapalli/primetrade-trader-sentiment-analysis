# 📊 Trader Performance vs Market Sentiment Analysis

## 🧠 Objective
This project analyzes how market sentiment (Fear/Greed) impacts trader behavior and performance using Hyperliquid trading data.

The goal is to uncover patterns that can inform smarter trading strategies.

---

## 📁 Datasets Used

### 1. Bitcoin Fear & Greed Index
- Columns: timestamp, value, classification, date
- Represents market sentiment (Fear, Greed, Extreme levels)

### 2. Hyperliquid Historical Trader Data
- 211,224 trade records
- Includes:
  - Account
  - Closed PnL
  - Size USD
  - Side (BUY/SELL)
  - Timestamp

---

## ⚙️ Methodology

### 🔹 Data Preparation
- Checked missing values and duplicates (none found)
- Converted timestamps to daily level
- Merged datasets using date
- Created key metrics:
  - `daily_pnl`
  - `win_rate`
  - `avg_trade_size`
  - `trades_per_day`
  - `long_ratio` / `short_ratio`

---

### 🔹 Data Characteristics
- Total trades: **211,224**
- Unique traders: **32**
- Unique trading days: **7**
- Final dataset: **102 trader-day observations**

> Note: Trading activity is highly concentrated on a few days.

---

## 📊 Key Insights

### 1. 📈 Higher Profitability During Fear
Traders achieve significantly higher average PnL during **Fear** conditions compared to Greed.

---

### 2. 🎯 Profit ≠ Higher Win Rate
Higher profitability is driven by **fewer large winning trades**, not higher win rates.

---

### 3. ⚡ Increased Activity in Extreme Markets
Trading frequency increases during extreme sentiment (Fear/Greed), indicating higher participation during volatility.

---

### 4. 💰 Larger Trade Sizes in Strong Sentiment
Traders take **larger positions** when sentiment is strong, indicating increased risk-taking behavior.

---

### 5. 🔄 Adaptive Positioning
Traders show a slight bias toward short positions, adjusting behavior based on market sentiment.

---

## 📊 Visualizations

The following charts are included:
- Average PnL by Sentiment
- Win Rate by Sentiment
- Trades per Day by Sentiment
- Trade Size by Sentiment
- Long vs Short Ratio

---

## 🎯 Strategy Recommendations

### ✅ Strategy 1: Trade Smart During Fear
- Participate actively
- Use controlled position sizing
- Avoid overexposure

---

### ⚠️ Strategy 2: Be Defensive During Extreme Greed
- Reduce trade frequency
- Avoid large positions
- Focus on high-confidence trades

---

## ⚠️ Limitations

- Data is limited to **7 trading days**
- Results should be interpreted as **directional insights**
- Not sufficient for strong causal conclusions

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
