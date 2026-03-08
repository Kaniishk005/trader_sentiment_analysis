# Trader Performance vs Market Sentiment Analysis

## Objective
Analyze how Bitcoin market sentiment (Fear vs Greed) affects trader behavior and profitability using Hyperliquid trading data.

## Dataset
1. Bitcoin Fear & Greed Index
2. Hyperliquid Historical Trader Data

## Methodology

1. Data Cleaning
   - Checked missing values and duplicates
   - Converted timestamps to datetime

2. Data Alignment
   - Aggregated trading data to daily level
   - Merged trader data with sentiment data

3. Feature Engineering
   - Win/Loss indicator
   - Trade size categories
   - Trader activity segmentation

4. Analysis
   - PnL vs Sentiment
   - Win Rate vs Sentiment
   - Long vs Short behavior
   - Trade size analysis

5. Trader Segmentation
   - Frequent vs Infrequent traders
   - K-Means clustering for behavioral archetypes

---
## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Key Insights

1. Trader profitability increases during Greed and Extreme Greed sentiment regimes.
2. Win rates are highest during Extreme Greed periods.
3. Traders slightly increase SELL positions during Extreme Greed markets.
4. Trade sizes are largest during Fear periods, suggesting opportunistic buying.
5. Infrequent traders outperform frequent traders, indicating overtrading may reduce profitability.

---

## Strategy Recommendations

**Strategy 1 — Momentum Trading**
- During Greed regimes traders may benefit from trend-following strategies.

**Strategy 2 — Opportunistic Buying**
- Fear periods show larger trade sizes and may present rebound opportunities.

---

## Bonus Analysis

K-Means clustering was applied to group traders based on:

- Average PnL
- Trade size
- Win rate

This identified three behavioral archetypes:

- Aggressive traders
- Conservative traders
- High-risk/high-reward traders

---

## How to Run
1. Clone the repository

```bash
git clone https://github.com/Kanishk005/trader_sentiment_analysis.git
cd trader_sentiment_analysis

2. Install required libraries
pip install -r requirements.txt

3. Launch Jupyter Notebook

4. Open the Notebook
notebooks/trader_sentiment_analysis.ipynb

5. Run all cells to reproduce the analysis and visualizations.

---

# What This Means Practically

A recruiter can do this:

```bash
git clone your_repo
pip install requirements
jupyter notebook