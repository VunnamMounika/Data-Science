# Data Science

#  Trader Behavior Analysis vs Bitcoin Market Sentiment

This project explores the relationship between trader performance and the Bitcoin market sentiment, using two datasets:

- `historical_data.csv` — Real trader data from the Hyperliquid platform
- `fear_greed_index.csv` — Daily Bitcoin Fear & Greed index

##  Objective

To uncover how trader behaviors like profitability, trade direction (BUY/SELL), and volume vary depending on market sentiment (e.g., Fear, Greed, Neutral), and deliver insights that can inform smarter trading strategies.

---

##  Datasets Used

1. Bitcoin Fear/Greed Index
   - Columns: `date`, `value`, `classification`
   - Classification includes: `Fear`, `Greed`, `Extreme Fear`, `Neutral`, etc.

2. Hyperliquid Historical Trader Data
   - Columns: `Timestamp IST`, `Account`, `Symbol`, `Execution Price`, `Side`, `Closed PnL`, `Leverage`, etc.

##  What This Notebook Does

- Loads and cleans both datasets
- Converts datetime formats to allow for merging
- Merges market sentiment with individual trade records
- Analyzes:
  - Average Closed PnL by sentiment
  - Number of trades by sentiment
  - BUY vs SELL distribution by sentiment
- Visualizes key insights using Seaborn
- Saves final merged dataset and summary for future use

##  Key Findings

- Traders earn the most on Extreme Greed days, but risk is also higher.
- Surprisingly, **Greed** days result in lower average profits than Fear days.
- Fearful markets see balanced BUY/SELL activity.
- Hidden Pattern: On Greed days, traders take more SELL positions than BUY.
- Insights like these can power sentiment-aware trading strategies.


##  Tools Used

- Python, Pandas, Matplotlib, Seaborn
- Jupyter Notebook
- Data source: Google Drive links provided in assignment

##  Files Included

- `data-analysis.ipynb` – Full code
- `merged_trader_sentiment.csv` – Cleaned data with sentiment matched
- `summary_by_sentiment.csv` – Summary report
