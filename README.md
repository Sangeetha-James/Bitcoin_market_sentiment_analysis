Trader Performance vs Market Sentiment (Fear vs Greed)

Role: Data Science / Analytics Intern
Company: Primetrade.ai
Candidate: Sangeetha

📌 Project Overview

This project analyzes how market sentiment (Fear vs Greed) influences trader behavior and performance on the Hyperliquid platform.
The objective is to identify behavioral patterns and derive actionable insights that can inform smarter trading strategies in Web3 markets.

📂 Repository Structure
ds_sangeetha/
├── notebook_1.ipynb        # Data loading, cleaning, feature engineering
├──                          # Analysis, visualization, insights
├── csv_files/
│   ├── fear_greed_index.csv
│   └── historical_data.csv
├── outputs/
│   ├── pnl_by_sentiment.png
│   └── summary_metrics_by_sentiment.csv
├── ds_report.pdf           # Final insights & strategy recommendations
└── README.md


⚠️ All notebooks were created and executed in Google Colab.

📊 Datasets Used
1. Bitcoin Market Sentiment Dataset

Columns: date, classification (Fear / Greed)

Source: Fear & Greed Index (provided)

2. Historical Trader Data (Hyperliquid)

Key fields:

account, coin, side

size_usd, closed_pnl

timestamp, trade_id

Source: Hyperliquid historical trade data (provided)

🛠️ Methodology
Part A — Data Preparation

Loaded and inspected both datasets

Checked for missing values and duplicates

Converted timestamps to daily granularity

Standardized column names

Aggregated trader-level daily metrics:

Daily PnL

Win rate

Trade count

Average trade size

Long/short ratio

Part B — Analysis

Merged trader metrics with daily sentiment data

Compared performance across Fear vs Greed days

Analyzed behavioral changes in:

Trading frequency

Position sizing

Segmented traders based on activity levels

Generated summary tables and visualizations

🔍 Key Insights

Higher profitability during Greed periods
Average daily PnL was higher during Greed days compared to Fear days, indicating more favorable trading conditions.

Overtrading during Fear reduces performance
High-activity traders experienced lower average PnL during Fear periods, suggesting overtrading under uncertainty.

Behavior changes more than skill
Win rates remained relatively stable across sentiments, while trade frequency and trade size varied significantly.

💡 Strategy Recommendations

Reduce trade frequency during Fear periods, especially for high-activity traders, to avoid overtrading losses.

Maintain disciplined position sizing during Greed periods instead of aggressively scaling trades.

📈 Outputs

Summary metrics by sentiment (summary_metrics_by_sentiment.csv)

PnL distribution by sentiment (pnl_by_sentiment.png)

Detailed insights and explanations in ds_report.pdf

▶️ How to Run

Open notebooks in Google Colab

Upload CSV files from the csv_files/ folder

Run notebook_1.ipynb first

 Outputs will be saved to the outputs/ folder

📎 Notes

All results are reproducible

No external datasets were used

Focus was on interpretability and actionable insights
