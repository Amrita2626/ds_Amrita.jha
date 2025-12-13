#Markdown
# ds_Amrita.jha
“Fear &amp; Greed Index + Trader Data Analysis”
# Trading Performance vs Market Sentiment

## Project Overview
This project analyzes cryptocurrency trading performance in relation to market sentiment using the **Fear & Greed Index**.
The objective is to understand how **fear and greed influence profitability, trading volume, volatility, and trader behavior**.

The analysis combines cleaned sentiment data with historical trading data to uncover actionable insights that can support
better trading strategy decisions.

---

## Datasets
The project uses two primary datasets:

1. **Fear & Greed Index**
   - Daily market sentiment values (0–100)
   - Classification such as Fear, Extreme Fear, Greed, Extreme Greed

2. **Historical Trading Data**
   - Executed cryptocurrency trades
   - Includes execution price, position size, PnL, fees, and trade direction

---

## Project Structure
project_root/
├── analysis.ipynb
├── csv_files/
│ ├── historical_cleaned.csv
│ ├── sentiment_cleaned.csv
│ └── merged_dataset.csv
├── outputs/
│ ├── analysis_summary.csv
│ ├── profit_by_sentiment.png
│ ├── volume_by_sentiment.png
│ ├── long_short_counts.png
│ ├── daily_profit.png
│ └── pnl_dist.png
├── reports/
│ └── ds_report.pdf
└── README.md




# Summary

---

## Data Processing Steps
1. Converted sentiment dataset UNIX timestamps to IST.
2. Cleaned and standardized sentiment classification labels.
3. Cleaned trader dataset numeric fields (PnL, size, execution price).
4. Created a common merge key using date alignment.
5. Merged sentiment and trading datasets using a left join.
6. Performed exploratory data analysis and visualization.

---

## Key Findings
- **Greed periods show a higher win rate** compared to fear periods.
- **Fear periods exhibit higher overall trading volume**, indicating increased activity during uncertainty.
- Trader behavior shifts significantly:
  - Fear → balanced long and short positions
  - Greed → increased short positions
- **Market volatility is higher during greed**, creating higher risk and reward opportunities.

---

## Conclusion
Market sentiment has a strong impact on trading performance and behavior.
Adapting trading strategies based on sentiment conditions can help traders
improve profitability while managing risk more effectively.

- Fear periods favor stable, risk-controlled strategies.
- Greed periods favor momentum strategies with stricter risk management.

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab
- GitHub

---

## Author
Amrita jha
