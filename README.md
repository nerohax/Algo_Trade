#  Algo-Trading Strategy with RSI, Moving Averages, and ML

A modular, backtestable algo-trading prototype built using Python, which:
- Applies RSI + Moving Average crossover strategy
- Fetches stock data using a free API
- Logs signals and P&L to Google Sheets
- Optionally includes ML to predict next-day movement

---

## 🔧 Features

### ✅ Core Logic
- **RSI < 30**: Identifies oversold conditions
- **20-DMA > 50-DMA**: Confirms bullish trend
- **Buy Signal**: Triggered when both conditions are true

### 📊 Technical Indicators
- RSI (Relative Strength Index)
- SMA20 & SMA50 (Simple Moving Averages)
- MACD (Moving Average Convergence Divergence)

### 📦 ML Automation (Optional)
- Predict next-day movement using indicators (RSI, MACD, Volume, etc.)
- Models supported: Logistic Regression, Decision Tree
- Displays accuracy

### 🧪 Backtesting Metrics
- Cumulative strategy return
- Sharpe ratio
- Win ratio
- Total return

### 📤 Google Sheets Integration
- Logs:
  - Trades
  - Strategy summary (P&L, win ratio)
- Organized into separate tabs

---

### Google Sheets Setup
- Create a service account via Google Cloud
- Share your Google Sheet with the service account email
- Save your credentials.json in the project directory

---

### 📚 Requirements
- Python 3.8+ , yfinance, ta, scikit-learn, gspread, oauth2client, pandas, matplotlib
