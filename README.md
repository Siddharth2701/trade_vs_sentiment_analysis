# Trader Behavior vs Market Sentiment Analysis

## 📌 Project Overview

This project analyzes how trader behavior changes under different market sentiment conditions using trading activity data and the Fear & Greed Index.

Instead of predicting prices, the goal is to understand **how trader psychology affects performance**.

The study examines whether traders make rational decisions or emotionally react during fear and greed phases of the market.

---

## 🎯 Objectives

* Measure trading behavior under different sentiment regimes
* Identify performance differences during fear vs greed markets
* Detect emotional trading patterns (overtrading, revenge trading, bottom catching)
* Segment traders based on risk and discipline
* Propose behavior-based trading rules to improve performance

---

## 📂 Dataset Description

### 1) Trading Data

Contains individual trade executions with:

* Account
* Timestamp
* Trade Side (Buy/Sell)
* Closed PnL
* Position Size (USD)

Used to calculate trader behavior metrics.

### 2) Sentiment Data

Fear & Greed Index with:

* Date
* Sentiment value
* Sentiment classification (Fear, Greed, etc.)

Used to measure market emotion.

---

## ⚙️ Methodology

### Step 1 — Data Preparation

* Converted timestamps to daily level
* Filtered closed trades
* Aggregated trades per trader per day

### Step 2 — Behavioral Metrics Created

* Daily PnL
* Win Rate
* Number of Executions
* Maximum Leverage Used
* Long/Short Ratio
* Drawdown Proxy (psychological pressure measure)

### Step 3 — Merge with Sentiment

Trader behavior aligned with market emotion on daily basis.

### Step 4 — Trader Segmentation

Traders categorized into behavioral groups:

* High vs Low leverage traders
* Frequent vs Infrequent traders
* Consistent vs Inconsistent performers

### Step 5 — Behavioral Analysis

Compared performance across:

* Fear vs Greed environments
* Different trader profiles

---

## 📊 Key Findings

1. **Fear causes overtrading**
   Trading activity increases significantly during extreme fear periods.

2. **Performance drops during fear**
   Win rate is lowest when traders trade the most.

3. **Leverage spikes in panic markets**
   Traders take highest risk during losses, indicating revenge trading behavior.

4. **Bottom catching bias**
   Traders aggressively go long during falling markets.

5. **Greed improves discipline**
   Higher win rates observed when traders trade less and follow trend.

---

## 🧠 Behavioral Insight

Losses are not primarily caused by market direction, but by emotional decision-making.

Traders perform worse when reacting to market moves and better when trading selectively.

---

## 📈 Strategy Rules Proposed

1. Reduce trading during extreme fear
2. Limit leverage during volatile conditions
3. Prefer trend-aligned trades in greedy markets

---

## 🛠 Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## ▶️ How to Run

1. Clone repository
2. Install requirements

```
pip install -r requirements.txt
```

3. Run notebook:

```
notebooks/analysis.ipynb
```

---

## 📎 Output

Charts demonstrate behavioral shift of traders across market sentiment conditions.

---

## 👤 Author

Data Analyst Candidate — Behavioral Finance Analysis Project
