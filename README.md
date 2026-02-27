# 📊 Prime Trade Intern Task

GitHub Repository: https://github.com/kavya-potnuru/prime-trade-intern-task

---

## 📌 Project Overview

This project analyzes trade-level data from a trading platform to understand trader behavior, performance, and sentiment-based effects.  
It implements trader segmentation and derives actionable insights that can be used to improve risk management and trading strategies.

---

## 🧠 Methodology

### 1️⃣ Data Aggregation  
Trade-level data was transformed into trader-level summaries, computing:

- Total number of trades  
- Average position size (USD)  
- Closed PnL (total and average)  
- Win rate (percentage of profitable trades)  
- Number of active trading days  

Data cleaning and preprocessing was done using pandas.

---

### 2️⃣ Trader Segmentation

Traders were categorized into segments:

- **Frequent vs Infrequent**  
  Based on trade count above/below the median

- **High Exposure vs Low Exposure**  
  Based on average position size

- **Consistent vs Inconsistent**  
  Based on win rate (win rate > 60% = consistent)

---

### 3️⃣ Behavioral and Performance Comparison

Each segment was compared on:

- Average PnL  
- Win rate  
- Position size  
- Trade frequency

Visualizations and tabular summaries were generated to support insights.

---

## 📈 Key Insights

### 🔹 Insight 1: Frequent Traders Drive Volume and Returns

- Frequent traders exhibit higher total PnL compared to infrequent traders.
- They also engage in more frequent activity and larger position sizes.

📊 Refer to: `chart_1.png`

---

### 🔹 Insight 2: Exposure Impacts Profitability

- High exposure traders show amplified PnL outcomes — both gains and losses.
- They have greater risk–return variability.

📊 Refer to: `chart_2.png`

---

### 🔹 Insight 3: Performance Dispersion Exists

- A subset of traders maintains a win rate above 60%, while many do not.
- Consistent winners generate more stable returns.

📄 Refer to: `table_1.png`  
📄 Refer to: `table_2.png`

---

## 🚀 Strategy Recommendations

### ✅ Strategy 1: Risk-Controlled Trading

**Rule of Thumb:**  
> Reduce leverage or position size for traders in the High Exposure and Inconsistent segment.

Rationale:  
This reduces drawdown risk and preserves capital for risk-averse segments.

---

### ✅ Strategy 2: Incentivize Consistent Performers

**Rule of Thumb:**  
> Allow higher trade frequency and more relaxed exposure constraints for consistent traders with moderate exposure.

Rationale:  
This encourages profitable trading behavior while managing risk.

---

## 🛠 Setup & How to Run

### Prerequisites

- Python 3.8+
- Recommended virtual environment

---

### Install Dependencies

```bash
pip install -r requirements.txt
