Financial Sentiment Analysis Project
📊 Project Overview
This project analyzes the correlation between financial news sentiment and stock market movements for Nova Financial Insights. The analysis aims to enhance predictive analytics capabilities and develop data-driven trading strategies.

🎯 Business Objective
Enhance financial forecasting accuracy by establishing statistical correlations between news sentiment and stock price movements, enabling predictive analytics for investment strategies.

📁 Project Structure
text
financial-sentiment-analysis/
├── .github/workflows/           # CI/CD pipelines
├── .vscode/                     # IDE settings
├── data/
│   ├── raw/                     # Original dataset (FNSPID)
│   └── processed/               # Cleaned and enriched data
├── notebooks/
│   ├── 01_eda_analysis.ipynb    # Task 1: Exploratory Data Analysis
│   ├── 02_technical_analysis.ipynb # Task 2: Quantitative Analysis
│   └── 03_correlation_analysis.ipynb # Task 3: Correlation Analysis
├── scripts/                     # Utility scripts
├── src/                         # Source code modules
├── tests/                       # Test cases
├── requirements.txt             # Python dependencies
└── README.md                   # Project documentation
🚀 Project Tasks
✅ Task 1: Git & GitHub + EDA (COMPLETED)
Repository Setup: Proper Git workflow with branching strategy

Exploratory Data Analysis:

Descriptive statistics and data quality assessment

Text analysis and topic modeling on headlines

Publisher and stock coverage analysis

Time series analysis of publication patterns

✅ Task 2: Quantitative Analysis (COMPLETED)
Technical Framework: Prepared for stock data integration

Data Processing: Cleaned and enriched news data

Analysis Preparation: Framework for correlation analysis

Processed Datasets: Ready for Task 3 implementation

🔄 Task 3: Correlation Analysis (IN PROGRESS)
Sentiment Analysis: NLP techniques on news headlines

Stock Integration: Merge with price data for correlation

Statistical Analysis: Establish sentiment-price relationships

Strategy Development: Trading insights and predictive models

📊 Dataset Information
FNSPID (Financial News and Stock Price Integration Dataset)
Total Articles: 1,351,341 financial news articles

Coverage Period: 2011-2024 (13-year span)

Unique Stocks: 6,204 companies

Unique Publishers: 1,034 news sources

Data Quality: 0 duplicates, 98.7% valid dates

Processed Data Files
news_analysis_ready.csv - Main analysis dataset with enriched features

daily_news_frequency.csv - Daily publication patterns

stock_daily_frequency.csv - Stock-specific coverage trends

top_stocks_analysis.csv - Selected stocks for detailed analysis

stock_coverage_statistics.csv - Comprehensive coverage metrics

analysis_summary.json - Project metadata and statistics

news_sample_10k.csv - Sample data for rapid testing

🛠️ Installation & Setup
Prerequisites
Python 3.8+

Git

Virtual environment (recommended)

Quick Start
bash
# Clone repository
git clone https://github.com/your-username/financial-sentiment-analysis.git
cd financial-sentiment-analysis

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter for analysis
jupyter notebook
Dependencies
Key Python packages:

pandas, numpy - Data manipulation

matplotlib, seaborn - Visualization

nltk, textblob - NLP and sentiment analysis

yfinance - Stock data integration

scikit-learn - Machine learning

📈 Key Findings (Interim Report)
Text Analysis Insights
Average Headline Length: 63.2 characters

Most Common Terms: "stock", "price", "earnings", "market", "shares"

Financial Categories: Earnings (18%), Price Movements (22%), Analyst Actions (15%)

Coverage Patterns
Top Stocks: AAPL, GOOGL, MSFT, AMZN, TSLA receive disproportionate coverage

Publisher Distribution: Power-law distribution with Reuters, Bloomberg, CNBC dominating

Temporal Patterns: Higher activity on weekdays, peaks during market hours

Data Quality
Success Rate: 98.7% of dates successfully parsed

Completeness: Minimal missing values across key columns

Consistency: Stable coverage throughout the 13-year period

🎯 Usage
Running Analysis
Start with EDA: Run notebooks/01_eda_analysis.ipynb for data exploration

Technical Preparation: Execute notebooks/02_technical_analysis.ipynb for quantitative framework

Correlation Analysis: Use notebooks/03_correlation_analysis.ipynb for final insights

Reproducing Results
python
# Load processed data for analysis
import pandas as pd
news_data = pd.read_csv('data/processed/news_analysis_ready.csv')
daily_freq = pd.read_csv('data/processed/daily_news_frequency.csv')
🤝 Contributing
Branch Strategy
main - Production-ready code

task-1 - EDA and initial analysis

task-2 - Quantitative analysis framework

task-3 - Correlation analysis and modeling

Commit Convention
feat: New features and functionality

fix: Bug fixes and corrections

docs: Documentation updates

analysis: Data analysis and insights

📋 Project Status
Task	Status	Completion Date
Task 1: EDA & Statistics	✅ Completed	Dec 2024
Task 2: Quantitative Analysis	✅ Completed	Dec 2024
Task 3: Correlation Analysis	🔄 In Progress	Target: Jan 2025
🎯 Next Steps
Immediate Priorities
Implement sentiment analysis using VADER and custom financial lexicons

Integrate historical stock price data for top 20 covered stocks

Establish statistical correlations between sentiment scores and price movements

Develop machine learning models for price prediction

Create interactive dashboards for strategy visualization

Expected Outcomes
Quantitative sentiment metrics for financial news

Statistical evidence of news-impact relationships

Actionable trading signals and strategies

Predictive models for stock price movements

