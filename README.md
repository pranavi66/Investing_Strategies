# 📈 Investing Strategies using Python

A quantitative investing project that demonstrates three popular investment strategies using real-time market data from Yahoo Finance. The project analyzes leading Indian stocks and builds portfolios based on different investment philosophies such as Equal Weight Investing, Value Investing, and Dividend Investing.

---

## 📖 Overview

Investing strategies play a crucial role in portfolio construction and wealth creation. This project showcases how Python can be used to automate stock analysis and portfolio selection using financial data.

The project implements three distinct approaches:

- **Equal Weight Investing** – Diversified portfolio allocation.
- **Value Investing** – Identification of potentially undervalued stocks.
- **Dividend Investing** – Selection of companies offering strong and sustainable dividend income.

The notebooks fetch market data, perform financial analysis, rank stocks, and suggest portfolio allocations.

---

## 🎯 Objectives

- Analyze Indian stock market data programmatically.
- Learn quantitative investing techniques.
- Build portfolios using different investment strategies.
- Perform financial ratio analysis.
- Automate stock screening using Python.

---

## 📂 Project Structure

```text
Investing_Strategies-main/
│
├── 01_equal_weights.ipynb
├── 02_value_investing.ipynb
├── 03_divident_investing.ipynb
├── top_50_indian_stocks.csv
└── README.md
```

### File Description

| File | Purpose |
|--------|---------|
| `01_equal_weights.ipynb` | Equal Weight Portfolio Strategy |
| `02_value_investing.ipynb` | Value Investing Stock Screener |
| `03_divident_investing.ipynb` | Dividend Investing Strategy |
| `top_50_indian_stocks.csv` | Top Indian Stocks Dataset |
| `README.md` | Project Documentation |

---

# 🚀 Strategy 1: Equal Weight Investing

## Concept

Equal Weight Investing allocates the same amount of capital to every stock in the portfolio regardless of market capitalization.

This ensures diversification and prevents overexposure to a single company.

### Workflow

1. Load stock symbols.
2. Fetch market data using Yahoo Finance.
3. Select target stocks.
4. Ask for investment amount.
5. Allocate equal capital to each stock.
6. Calculate the number of shares to purchase.

### Example

Portfolio Value:

```text
₹100,000
```

Number of Stocks:

```text
10
```

Investment per Stock:

```text
₹100,000 ÷ 10 = ₹10,000
```

### Advantages

- Simple portfolio construction.
- Broad diversification.
- Easy to understand and implement.

---

# 💰 Strategy 2: Value Investing

## Concept

Value Investing seeks stocks that are trading below their intrinsic value.

The notebook evaluates companies using multiple valuation metrics and ranks them according to a composite value score.

### Financial Ratios Used

#### Price-to-Earnings (P/E)

```text
P/E = Price / Earnings
```

Measures how much investors are willing to pay for each unit of earnings.

---

#### Price-to-Book (P/B)

```text
P/B = Market Price / Book Value
```

Compares company valuation with its net assets.

---

#### Price-to-Sales (P/S)

```text
P/S = Market Capitalization / Revenue
```

Measures valuation relative to company sales.

---

#### EV/EBITDA

Enterprise value relative to operating earnings.

---

#### EV/Gross Profit

Measures company value relative to gross profit.

---

### Value Score Calculation

Each metric is converted into percentile rankings.

Final score:

```text
Value Score =
Average(
PE Percentile,
PB Percentile,
PS Percentile,
EV/EBITDA Percentile,
EV/GP Percentile
)
```

Stocks with the highest scores are considered attractive value opportunities.

### Advantages

- Data-driven stock selection.
- Uses multiple valuation metrics.
- Reduces dependency on a single ratio.

---

# 💵 Strategy 3: Dividend Investing

## Concept

Dividend investing focuses on companies that consistently return profits to shareholders through dividend payments.

The strategy evaluates both dividend strength and sustainability.

### Metrics Used

#### Dividend Yield

```text
Dividend Yield =
Annual Dividend / Share Price
```

Measures dividend income generated per unit of stock price.

---

#### Dividend Rate

Annual dividend paid per share.

---

#### Payout Ratio

```text
Payout Ratio =
Dividends / Earnings
```

Indicates how much of earnings are distributed as dividends.

---

#### Dividend Growth

Measures historical dividend growth.

---

#### Earnings Growth

Ensures future dividend sustainability.

---

### Weighted Scoring Model

| Metric | Weight |
|----------|---------|
| Dividend Yield | 30% |
| Dividend Rate | 20% |
| Payout Ratio | 20% |
| Dividend Growth | 20% |
| Earnings Growth | 10% |

Final score:

```text
Dividend Score =
0.30 × Yield +
0.20 × Dividend Rate +
0.20 × Payout Ratio +
0.20 × Dividend Growth +
0.10 × Earnings Growth
```

Stocks are ranked based on the overall dividend score.

### Advantages

- Focus on passive income.
- Prioritizes financially healthy companies.
- Suitable for long-term investors.

---

# ⚙️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- SciPy
- yFinance
- Financial Data Analysis

---

# 📊 Workflow

```text
                Top 50 Indian Stocks
                         │
                         ▼
                Yahoo Finance API
                         │
                         ▼
                 Financial Data
                         │
       ┌─────────────────┼─────────────────┐
       │                 │                 │
       ▼                 ▼                 ▼
 Equal Weight      Value Investing   Dividend Investing
       │                 │                 │
       ▼                 ▼                 ▼
 Portfolio         Stock Ranking     Dividend Ranking
 Construction
       │                 │                 │
       └────────────► Results ◄────────────┘
```

---

# 📦 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Investing_Strategies.git
cd Investing_Strategies
```

Install dependencies:

```bash
pip install pandas numpy scipy yfinance jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open any notebook and run the cells sequentially.

---

# 📈 Learning Outcomes

By completing this project, you will learn:

- Portfolio construction techniques
- Quantitative investing concepts
- Financial ratio analysis
- Value investing methodology
- Dividend investing methodology
- Data collection using Yahoo Finance
- Python-based stock screening

---

# 🔮 Future Improvements

- Portfolio backtesting
- Risk management metrics
- Sharpe Ratio analysis
- Portfolio optimization
- Rebalancing strategies
- Streamlit dashboard
- Machine learning-based stock ranking

---

# ⚠️ Disclaimer

This project is intended for educational and learning purposes only. It should not be considered financial advice. Always conduct your own research before making investment decisions.

---

