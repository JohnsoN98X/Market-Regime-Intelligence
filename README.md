# 🧠 Market Regime Modeling, Analysis, and Forecasting

This project focuses on identifying, analyzing, and forecasting **market regimes** using a pipeline that combines unsupervised learning, anomaly detection, Markov modeling, and supervised classification. The goal is to uncover structural market behavior and enable regime-aware decision-making.

## 📁 Project Structure

- **01_Regime_Classification**  
  Identification of market regimes using the KMeans algorithm, followed by statistical analysis and characterization of each regime. Also includes PCA-based dimensionality reduction and visualization.

- **02_Anomaly_Detection**  
  Global and local anomaly detection using Isolation Forest and LOF, applied both to the full dataset and within each market regime cluster.

- **03_Markov_Chain.ipynb**  
  Modeling regime transitions using a discrete-time Markov chain. Includes transition matrix estimation, stationary distribution, multi-step transition probabilities, expected duration in each regime, and more.

- **04_XGBC_Regime_Prediction.ipynb**  
  Training an XGBoost classifier (XGBC) to forecast market regimes. Hyperparameters are tuned using Optuna for efficient search.

## 🧪 Libraries Used

- `numpy`, `pandas`, `scipy`
- `matplotlib`, `seaborn`
- `sklearn`, `optuna`
- `yfinance`

## 📊 Data Source

- Market data is downloaded programmatically using `yfinance`.

## ▶️ How to Run

1. Clone the repo and install dependencies:  
   `pip install -r requirements.txt`

2. Run notebooks in order:  
   `01 → 02 → 03 → 04`

## 📁 Folder Structure

```
notebooks/        ← All Jupyter notebooks (01–04)
data/             ← Cleaned and raw financial datasets
README.md         ← Project documentation
```

## 📈 Output

Final output includes:
- Visualized market regimes
- Anomaly flags (global + per-regime)
- Markovian regime behavior
- Forecasting model for real-time regime prediction

## 📄 License

This project is licensed under the MIT License.
