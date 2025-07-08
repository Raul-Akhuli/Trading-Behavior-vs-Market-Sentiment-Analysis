# 📊 Trading Behavior vs Market Sentiment Analysis

This project analyzes how trading behavior (profitability, volume, risk, number of trades) aligns or diverges from the overall market sentiment (Fear & Greed Index). The goal is to identify hidden patterns and actionable insights for smarter trading strategies.

---

## 📁 Datasets Used

1. **historical_data.csv**  
   - Trade-level records including:
     - Execution Price
     - Trade Volume
     - PnL (Profit & Loss)
     - Fees, Timestamp, Direction, etc.

2. **fear_greed_index.csv**  
   - Daily market sentiment score:
     - `value`: Ranges from 0 (Extreme Fear) to 100 (Extreme Greed)
     - `classification`: Label of market mood (e.g., Fear, Greed)

---

## 🛠️ How to Run

### 1. Requirements

Make sure the following Python libraries are installed:

```bash
pip install pandas matplotlib seaborn fpdf
```

### 2. Running the Analysis

Use the provided Python script or Jupyter Notebook to:

- Load and clean both datasets
- Merge them on the `date` field
- Compute daily trading metrics:
  - Total PnL
  - Total Volume (USD)
  - Number of Trades
  - Average Execution Price
  - Total Fees
- Correlate with the sentiment score
- Visualize insights using:
  - Correlation heatmaps
  - Boxplots for sentiment classification vs PnL/volume

---

## 📈 Output

- `merged_trading_sentiment_data.csv`: Cleaned and combined dataset
- `Trading_Sentiment_Report.pdf`: Full insights and strategy notes
- Visualizations: Heatmaps and boxplots showing behavior vs sentiment

---

## 💡 Key Insights

- Trading activity increases during *Greed* phases — but profits do **not**.
- Traders show better risk management and outcomes during *Fear*.
- The Fear & Greed Index can be used as a **filter** for:
  - Avoiding overtrading during hype
  - Identifying calm entry points after panic selling

---

## 📝 Notes

- Ensure timestamps are in consistent format before analysis.
- You may enrich the analysis by adding:
  - Leverage metrics
  - Coin-wise performance trends
  - Win/Loss ratio or drawdown

---

## 👤 Author

**Raul Akhuli**  
Specialization: AI & ML | CSE | [Kolkata, India]  
Love for data, teaching, and intelligent strategy design.
