# Hourly Energy Consumption Forecasting with XGBoost

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![XGBoost](https://img.shields.io/badge/XGBoost-1.5+-orange.svg)](https://xgboost.ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Overview

This project builds a production-ready time series forecasting model to predict hourly energy consumption for the PJM interconnection grid. Using XGBoost with engineered temporal features and lag variables, the model achieves **89% accuracy** and significantly outperforms naive baselines.

**Business Value**: Accurate load forecasting enables grid stability, optimized power purchasing, and reduced operational costs. A 1% improvement in forecast accuracy can save millions annually.

---

## Key Results

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **Model Accuracy** | 89.1% | Predictions within 11% of actual values |
| **RMSE** | ~3,456 MW | Average prediction error |
| **vs Baseline** | 29.3% better | Outperforms "same hour last week" forecast |
| **Top Features** | Month (31%), Hour (29%) | Model learns real seasonal & daily patterns |

---

## 🛠️ Technologies Used

- **Python** - Core programming language
- **Pandas/NumPy** - Data manipulation and analysis
- **XGBoost** - Gradient boosting for regression
- **Scikit-learn** - Time series cross-validation, metrics
- **Matplotlib/Seaborn** - Data visualization

---
## Installation & Usage

```bash
# Clone the repository
git clone https://github.com/nushyiscoding/energy-forecast-xgboost.git

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook energy_forecast.ipynb
