# Quantitative Trading Strategy - Inter IIT Tech Meet Submission

This project showcases a **quantitative trading strategy** developed for the **Inter IIT Tech Meet**. The notebook includes feature engineering, alpha generation using technical indicators, and model training to build a predictive model for stock price movements.

## 📁 Project Structure

```
quant_inter_iit_final_notebook.ipynb  
```

## 🚀 Objective

The goal is to:

* Build a predictive model that forecasts future price movements based on engineered features.
* Use historical stock price data to derive alpha factors using a variety of technical indicators.
* Backtest the effectiveness of different strategies using machine learning models.

---

## 📊 Features & Techniques

### ✅ Data Preprocessing

* Stock price data is read and missing values are handled appropriately.
* Volatility measures and log returns are computed to represent price action.

### 🧠 Feature Engineering

* **Technical indicators**: Includes RSI, MACD, Bollinger Bands, ATR, OBV, etc.
* **Momentum & mean-reversion signals**: Designed to capture short- and long-term trading signals.

### 📈 Alpha Generation

* Signal-based labeling: 'Buy', 'Hold', and 'Sell' labels are generated using future returns and volatility thresholds.
* Balanced the dataset to prevent class imbalance.

### 🤖 Model Training

* Used `XGBoost` for classification.
* Evaluated using confusion matrix, classification report, and precision scores.
* Hyperparameter tuning with `GridSearchCV`.

### 📉 Strategy Evaluation

* Strategy performance evaluated on test data.
* Predictions are mapped to trading decisions.
* Cumulative returns plotted and compared against market returns.

---

## 🛠️ Requirements

Install the necessary dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost ta
```

---

## 📌 How to Run

1. Clone the repository or download the notebook.
2. Install required packages.
3. Run all cells in `quant inter iit final notebook.ipynb`.
4. Analyze model outputs and cumulative return plots.

---

## 📈 Sample Results

* Confusion matrix showing precision and recall for each label.
* Strategy return plots outperforming or aligning with baseline.
* Importance of technical indicators for model decisions.

---

## 🧠 Insights

* Feature importance reveals that **MACD**, **RSI**, and **Bollinger Band width** were key drivers of model decisions.
* Ensemble methods like XGBoost provided superior results over baseline classifiers.
* Strategy is sensitive to volatility-based labeling.

---

## 📚 References

* [Technical Analysis Library in Python (TA-Lib)](https://technical-analysis-library-in-python.readthedocs.io/en/latest/)
* [XGBoost Documentation](https://xgboost.readthedocs.io/)
* Quantitative finance blogs and research papers on alpha generation

---

## 🏁 Final Notes

This project demonstrates how machine learning can be used to derive trading insights from historical stock data. It is intended as an academic prototype and is **not financial advice**.
