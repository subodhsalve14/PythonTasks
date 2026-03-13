

## 📌 Project Overview

This project explores the relationship between **Cryptocurrency Trading Performance** (PnL) and **Market Sentiment** (Fear & Greed Index). By merging historical trade data with daily sentiment scores, this analysis identifies whether market emotions—ranging from "Extreme Fear" to "Extreme Greed"—act as leading or lagging indicators of trader profitability.

## 🚀 Key Features

* **Automated Data Merging:** Intelligent timestamp alignment between high-frequency trading logs and daily sentiment data.
* **Robust Column Mapping:** Built-in "Automatic Column Detector" to handle variations in CSV naming conventions (e.g., `PnL` vs `Closed_PnL`).
* **Sentiment Correlation:** Analysis of how different market cycles (Fear vs. Greed) impact win rates and average profitability.
* **Reversal Analysis:** Lagged data modeling to determine if yesterday’s sentiment predicts today's market performance.
* **Signal Generation:** An algorithmic trading strategy that generates `BUY`, `SELL`, or `HOLD` signals based on Extreme Fear/Greed thresholds.

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:** * `Pandas`: Data manipulation and time-series merging.
* `NumPy`: Mathematical operations.
* `Matplotlib` & `Seaborn`: Statistical data visualization and heatmaps.


* **Platform:** Google Colab / Jupyter Notebook

## 📊 Analysis Highlights

### 1. Market Sentiment Performance

The analysis categorizes trades into five sentiment zones.

* **Greed:** Often correlates with higher total PnL but requires strict exit strategies.
* **Fear:** Historically represents a "BUY" opportunity with a distinct recovery PnL pattern.

### 2. Strategy Backtest Results

The system evaluates a simple sentiment-based strategy:

* **Signal - BUY:** Triggered during "Extreme Fear" (Sentiment Score $\le$ 1).
* **Signal - SELL:** Triggered during "Extreme Greed" (Sentiment Score $\ge$ 3).

### 3. Correlation Heatmap

A visual matrix exploring the strength of the relationship between the **Sentiment Score**, **PnL**, and **Win Rate**.

## 📂 File Structure

* `Python_Task.ipynb`: The main execution notebook containing data cleaning, merging, and visualization.
* `historical_data.csv`: Source file for trader execution logs (Account, Coin, PnL, etc.).
* `fear_greed_index.csv`: Daily sentiment scores and classifications.
* `Subodh_Salve_Trading_Analysis.csv`: The final engineered dataset with signals and merged metrics.



