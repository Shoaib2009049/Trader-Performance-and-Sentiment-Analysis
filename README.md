📊 Bitcoin Market Sentiment vs Trader Performance
This project explores how market sentiment (Fear & Greed Index) influences trader performance, using real-world datasets that include both Bitcoin sentiment data and historical trader activity from Hyperliquid.

📁 Datasets Used
Fear & Greed Index

Columns: date, classification (Extreme Fear → Extreme Greed), value
Represents daily market sentiment toward Bitcoin
Hyperliquid Historical Trader Data

Includes: account, execution price, side (buy/sell), size USD, closed PnL, timestamp, etc.
Represents individual trades executed by traders
🎯 Objective
To explore the relationship between trader behavior/performance and market sentiment, uncover hidden patterns, and deliver actionable trading insights.

🧠 Key Steps Performed
Data Cleaning & Preprocessing

Standardized and merged both datasets using date
Encoded sentiment levels (Extreme Fear → 0, ... Extreme Greed → 4)
Filtered and retained relevant trade columns
Feature Engineering

Trade-Level Metrics:
PnL_bin (Profit/Loss)
Side_Binary (Buy = 1, Sell = 0)
Normalized PnL (P&L adjusted by trade size)
Account-Level Daily Aggregates:
Total PnL, Profit Rate, Buy Ratio, Avg Trade Size, etc.
Analysis & Visualization

Used seaborn/matplotlib to analyze patterns across sentiment classes
Created boxplots and summaries to evaluate shifts in performance and behavior
📊 Summary of Findings
🔹 Performance Metrics Vary with Sentiment
Traders perform significantly better during Greed and Extreme Greed
Fear periods lead to more losses and lower average PnL
🔹 Trade Direction is Sentiment-Driven
Buy-side trades dominate in Greed
Sell/Short trades become more frequent during Fear
🔹 Risk-Taking Behavior Shifts with Sentiment
Larger trade sizes and higher trade volumes observed in Greed
Traders are more conservative during Fear phases
🔍 Meaningful Insights & Recommendations
✅ For Traders
Use sentiment as a filter: Avoid overtrading during Fear
Leverage momentum in Greed phases but manage risk
✅ For Algorithmic Strategy Design
Include sentiment_score as a feature in ML models
Dynamic position sizing or stop-loss logic based on sentiment
✅ For Analysts / Firms
Monitor performance segmented by sentiment
Identify traders who outperform during fear — potential contrarians or mean-reverters
🚀 Next Steps (Optional Ideas)
Build a Streamlit dashboard for live sentiment-trader analysis
Run clustering to categorize trader personas
Train a model to predict profitable trades using sentiment + trade features

📌 Conclusion
This analysis demonstrates that market sentiment significantly impacts trader performance and behavior. By quantifying this relationship, we can design smarter trading strategies, improve risk management, and enable context-aware decision-making in volatile crypto markets.
