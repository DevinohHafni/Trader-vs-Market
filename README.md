# Trader-vs-Market
Analyzing how market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid

# Trader Performance vs Market Sentiment — Primetrade.ai Assignment

## Setup
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

## How to Run
jupyter notebook notebook.ipynb
Run all cells top to bottom

## Project Structure
primetrade_assignment/
├── data/
│   ├── sentiment.csv
│   └── trades.csv
├── charts/
│   ├── full_analysis.png
│   ├── elbow.png
│   └── clusters.png
├── notebook.ipynb
└── README.md

## Methodology
- Merged 211,224 trades with Fear/Greed sentiment index by date
- Engineered key metrics per trader and per day
- Segmented traders into 3 behavioral dimensions
- Random Forest model: 95% accuracy predicting daily profitability
- K-Means clustering: 4 trader archetypes identified

## Key Insights
1. Traders are 2.3x more active on Fear days — panic trading behavior
2. Greed days produce more consistent profits despite similar average PnL
3. Sentiment alone has minimal predictive power (0.6%) — trader behavior dominates
4. Large traders profit more during Fear; Mid traders thrive on Greed days
5. Steady Winners cluster: highest win rate (50%), lowest drawdown (-$11K)

## Strategy Recommendations
1. Large position traders → hold or increase size on Fear days
2. Mid size traders → increase activity and size on Greed days
3. All traders → focus on win rate consistency over volume

## Bonus
- Random Forest classifier: 95% accuracy
- K-Means clustering: 4 archetypes (Blown Account, High Risk Gamblers, Power Traders, Steady Winners)
