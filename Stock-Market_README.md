# Stock Market Performance Analysis

A data analysis project that pulls **real-time historical stock data** using the `yfinance` API and visualises the performance of major tech companies over the last 3 months using interactive Plotly charts.

---

## 📌 Project Overview

This project analyses and compares the stock market performance of 4 major tech companies — **Apple, Microsoft, Netflix, and Google** — using live financial data fetched directly from Yahoo Finance.

**Key Questions Answered:**
- How did each stock perform over the last 3 months?
- Which stock showed the strongest growth?
- What are the price trends, highs, lows, and trading volumes?

---

## 📊 Companies Analysed

| Ticker | Company |
|---|---|
| `AAPL` | Apple Inc. |
| `MSFT` | Microsoft Corporation |
| `NFLX` | Netflix Inc. |
| `GOOG` | Alphabet Inc. (Google) |

**Data Period:** Last 3 months (dynamically fetched at runtime)

---

## 📈 Data Features

| Column | Description |
|---|---|
| `Ticker` | Stock symbol |
| `Date` | Trading date |
| `Open` | Opening price |
| `High` | Daily high price |
| `Low` | Daily low price |
| `Close` | Closing price |
| `Adj Close` | Adjusted closing price |
| `Volume` | Number of shares traded |

---

## 🔧 Analysis Workflow

1. **Install & Import Libraries** — `yfinance`, `pandas`, `plotly`
2. **Fetch Live Data** — Download last 3 months of OHLCV data for all 4 tickers using `yfinance`
3. **Data Wrangling** — Concatenate multi-ticker DataFrames, reset index
4. **Interactive Visualisation** — Plot closing price trends per ticker using Plotly Express line charts
5. **Performance Comparison** — Compare price movements across all 4 stocks on a single chart

---

## 📉 Sample Price Snapshot (March–June 2023)

| Ticker | Start Price (~) | End Price (~) | Trend |
|---|---|---|---|
| AAPL | $151 | $181 | 📈 +20% |
| MSFT | $255 | $335 | 📈 +31% |
| NFLX | $315 | $400 | 📈 +27% |
| GOOG | — | — | 📈 Upward |

> Prices fetched dynamically — run the notebook to get the latest 3-month window.

---

## 🛠️ Tech Stack

- Python 3.x
- Pandas
- yfinance
- Plotly Express
- datetime

---

## 📁 Project Structure

```
Stock-Market-Performance-Analysis/
│
└── Code/
    └── Stock_Market_Performance_Analysis.ipynb   # Full analysis notebook
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install yfinance pandas plotly
```

### Run the Notebook

```bash
jupyter notebook Code/Stock_Market_Performance_Analysis.ipynb
```

> **Note:** An active internet connection is required — the notebook fetches live data from Yahoo Finance at runtime.

---

## 🔍 Key Concepts Demonstrated

- **Live Data Fetching** — Using `yfinance` to pull real financial data via API
- **Multi-ticker Analysis** — Combining data from multiple stocks into a single DataFrame
- **Interactive Visualisation** — Plotly line charts with hover, zoom, and pan
- **Time Series Analysis** — Tracking price movements over a 3-month window
- **Comparative Analysis** — Side-by-side performance of multiple companies

---

## 👤 Author

**Osho Muralidaran**  
[LinkedIn](https://www.linkedin.com/in/osho-m) · [GitHub](https://github.com/osho-m)
