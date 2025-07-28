# Market Regime Detection and Forecasting

## 📌 Project Description

This project focuses on the detection, analysis, and advanced forecasting of market regimes.  
Market regimes are distinct periods in financial markets characterized by changes in statistical behavior, such as volatility, momentum, and correlations. Identifying these regimes is essential for building adaptive strategies, managing risk, and understanding market structure.

---

## 🎯 Objective

To deepen and showcase personal expertise in quantitative financial analysis, financial theory, statistics, mathematics, stochastic processes, and advanced Python programming through a full-cycle market regime modeling project.

---

## 🧱 Project Structure

### Part I: Regime Detection and Characterization
- Unsupervised learning with **KMeans** clustering.
- Dimensionality reduction using **PCA**.
- Statistical testing and interpretation of regime-specific characteristics.

### Part II: Anomaly Detection
- **Global anomaly detection** using Isolation Forest.
- **Local anomaly detection** within each regime using **LOF**.
- Final global consistency check.

### Part III: Markov Chain Modeling
- Transition matrix construction.
- Stationary distribution calculation.
- Transition probability analysis across time.
- Sojourn time and expected return time analysis.

### Part IV: Regime Forecasting
- Supervised models trained on past 7-day windows:
  - **Ridge Classifier**
  - **XGBoost Classifier (XGBC)**
- Advanced hyperparameter optimization with **Optuna**.

---

## 📊 Results

- Statistically distinct market regimes were successfully identified.
- Global and local anomalies were consistently detected.
- Markov chain modeling revealed meaningful regime dynamics.
- An XGBoost model was built with strong predictive capability for market regime classification.

---

## 🧠 Future Directions

- Integration of **Explainable AI (XAI)** tools (e.g. SHAP) to interpret feature influence on regime prediction.
- Development of a specialized model for detecting "panic" regimes, which showed weaker predictive performance compared to others.

---

## 🗂️ Data Source

- Data retrieved from **Yahoo Finance** using the `yfinance` API.
- All processing and modeling performed **locally** for full control and custom analysis.

---

## ⚙️ Requirements

Install dependencies with:
```bash
pip install -r requirements.txt
```

Or install manually:
```bash
pip install pandas numpy scipy matplotlib seaborn xgboost scikit-learn yfinance optuna
```

---

## 🚀 Quick Start

Example usage:
```bash
python main.py --mode full_run
```

Steps:
1. Extract data from Yahoo Finance.
2. Run regime clustering and PCA visualization.
3. Detect anomalies globally and locally.
4. Model regime transitions with a Markov chain.
5. Train and evaluate machine learning models for regime prediction.

---

## 📄 License

This project is released under the MIT License.

---

## ⚠️ Disclaimer

This project is for educational and research purposes only.  
Any use of the code or insights for financial decision-making is entirely at your own risk.  
The author assumes no responsibility for any outcomes resulting from its use.


```
*This project combines unsupervised learning, anomaly detection, stochastic modeling, and supervised forecasting to create a comprehensive market regime analytics pipeline.*
