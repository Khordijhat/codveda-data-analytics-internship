# Codveda Data Analytics Internship

Projects completed during my Data Analytics internship at **Codveda**, using Python to analyze social media, stock price, and trading data.

## Projects (Level 2)

| Task | Topic | Dataset | Techniques |
|---|---|---|---|
| 1 | Regression Interpretation | Social media sentiment data | Simple and multiple linear regression, train/test split, R² and MSE |
| 2 | Time Series Analysis | Stock prices (AAL) | Seasonal decomposition, 20-day and 50-day moving averages |
| 3 | K-Means Clustering | Stock prices (AAL) | Feature scaling, Elbow Method, K-Means, outlier detection |

## Key Findings

**Task 1: Regression**
- Posting hour has a weak positive relationship with likes (about 0.75 more likes per hour), but it explains under 5% of the variance and does not generalize to new data (test R² is negative).
- Every post in the dataset has exactly two hashtags, so the effect of hashtag count could not be tested.
- Neither feature is a reliable linear predictor of likes.

**Task 2: Time Series**
- AAL's price moved in multi-month trends, between roughly $25 and $55 from 2014 to 2018.
- The weekly seasonal component is negligible (about ±$0.03), so there is no meaningful day-of-week pattern.
- The 20-day and 50-day moving average crossovers matched the major upward and downward phases.

**Task 3: Clustering**
- Trading days split mainly into lower-price and higher-price groups, separated at around $42–45.
- The model isolated one extreme-volume day (about 138 million shares) as its own cluster, showing how clustering can flag unusual market activity.

## Tools Used
Python · pandas · NumPy · Matplotlib · scikit-learn · statsmodels · Jupyter Notebook

## Repository Structure
```
codveda-data-analytics-internship/
├── README.md
└── level-2/
    ├── codveda_level2.ipynb
    ├── sentiment.csv
    └── stock_prices.csv
```
## Data
The datasets were provided by Codveda as part of the internship.
- `sentiment.csv`: social media posts with sentiment, hashtags, likes, retweets, and timestamps
- `stock_prices.csv`: daily open, high, low, close, and volume for multiple stock symbols (the analysis uses AAL)

## Limitations
- Task 1: the hashtag feature had no variation, and the models used different random splits, so the metrics are indicative and not strictly comparable.
- Tasks 2 and 3 analyze a single stock (AAL) and do not generalize to the full dataset.
- This is an educational analysis and not financial advice.

## Author
**FAJOBI ADIJAT OLUWATOYIN**
Data Analyst
[LinkedIn](https://www.linkedin.com/in/adijat-fajobi) · [Upwork](https://www.upwork.com/freelancers/adijat-fajobi)
