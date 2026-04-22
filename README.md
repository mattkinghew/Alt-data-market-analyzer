# 📈 Alt-Data Market Insight Agent

## 🎯 Project Overview
The **Alt-Data Market Insight Agent** is a lightweight analytics engine designed to bridge the gap between traditional quantitative finance and modern alternative data. It combines historical price actions (technical indicators) with alternative data streams (e.g., social media sentiment) to provide automated, robust market risk assessments.

## 💡 Business Value (The "Why")
Traditional financial models heavily rely on historical prices, which often lag during black-swan events or sudden macroeconomic shifts. Quantitative analysts face the challenge of extracting signal from the noise.
This solution:
1. **Reduces Overfitting:** Utilizes K-Fold Cross Validation to ensure that selected technical indicators remain robust across different market regimes.
2. **Captures Non-Rational Volatility:** Integrates Alternative Data (Social Media Sentiment & Volume) as a leading indicator to capture retail investor psychology.
3. **Automates Insight:** Lays the groundwork for an automated workflow that translates raw data into executive-level risk briefings.

## 🛠️ Technical Architecture
This project is modularized into distinct data pipelines:
- **Data Ingestion Layer:** Fetches real-time ETF data (e.g., IVV) via `yfinance` API and handles simulated non-structured sentiment data.
- **Feature Engineering Layer:** Dynamically calculates Moving Averages (SMA) and Momentum indicators.
- **Validation Layer:** Implements 5-Fold Cross Validation alongside Pearson Correlation to evaluate feature predictive power while strictly preventing look-ahead bias.

## 🚀 Future Roadmap
To evolve this project from an analytical script into a fully autonomous AI Agent, the following modules are planned:
- [ ] **LLM Integration:** Feed the EDA statistical outputs into an LLM (GPT-4/Gemini) to automatically generate daily "Morning Risk Briefings".
- [ ] **Workflow Automation:** Orchestrate the data pipeline using **n8n** or **Make.com** for daily scheduled execution.
- [ ] **Interactive Dashboard:** Wrap the Python logic into a **Streamlit** web application for intuitive data exploration.

## 💻 Getting Started
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the analysis within the `notebooks/` directory.
