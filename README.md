# 📊 Stock Market KPI Dashboard

An automated pipeline and dashboard that track multi-stock performance over time.  
Built with **Python**, **yfinance**, and **Power BI**, this project calculates and visualizes key performance indicators (KPIs) such as volatility, Sharpe ratio, and moving averages.

---

## 🚀 Project Overview

**Goal:** Build an automated financial dashboard that helps analyze stock risk and return over a 2-year window.

**Key Features**
- Fetches historical price data using `yfinance`
- Calculates:
  - Daily returns
  - Annualized volatility
  - Sharpe ratio (risk-adjusted return)
  - 50-day and 200-day moving averages
- Generates clean CSVs for Power BI
- Includes Power BI visuals for:
  - Price trends
  - Volatility comparison
  - Return vs. risk (Sharpe ratio)
  - KPI summary cards

---

## 🧩 Tech Stack

| Layer | Tool |
|-------|------|
| Data Source | Yahoo Finance API (`yfinance`) |
| Processing | Python (`pandas`, `numpy`) |
| Visualization | Power BI Desktop |
| Storage | Local CSV (offline mode) |
| Future Hosting | Power BI Service / Streamlit Cloud |

---

## 📂 Project Structure
stock-kpi-dashboard/
│
├── src/ # Python scripts
├── data/ # Generated CSV outputs
├── visuals/ # Power BI file & screenshots
├── notebooks/ # Optional EDA notebooks
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE

---

## 🧮 How It Works

1. **Run the Python script** to fetch and process data:
   ```bash
   python src/build_kpis.py --tickers AAPL MSFT TSLA NVDA --period 2y --interval 1d --out ./data/kpis.csv
