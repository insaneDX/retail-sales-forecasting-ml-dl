# Retail Sales Forecasting using Machine Learning & Deep Learning

This repository contains an **end-to-end time series forecasting project** for retail store sales using **Machine Learning and Deep Learning models**.  
The project focuses on the **Rossmann Store Sales dataset** and demonstrates how different modeling approaches perform on the same forecasting problem.

---

## Problem Statement

Retail sales forecasting is a classic **time series prediction problem** where future sales depend on:
- Historical sales
- Seasonality and trends
- Store-specific patterns
- Calendar effects (day, week, month)

The goal of this project is to **compare traditional ML models and modern deep learning models** for sales forecasting.

---

## Models Implemented

The following models are implemented and compared:

- **XGBoost**
  - Uses lag features and rolling statistics
  - Strong baseline for tabular time-series data

- **Prophet**
  - Captures trend and seasonality explicitly
  - Designed for business forecasting use-cases

- **LSTM (Long Short-Term Memory)**
  - Recurrent neural network for sequential data
  - Learns temporal dependencies automatically

- **Transformer**
  - Attention-based deep learning model
  - Handles long-range temporal dependencies efficiently

---

## Repository Structure

```

retail-sales-forecasting-ml-dl/
│
├── README.md
├── EDA_&_Feature_Engineering_for_Rossmann_Store_Sales.ipynb
├── modelling-for-rossmann-store-sales-1.ipynb
├── modelling-for-rossmann-store-sales-2-transformer.ipynb

````

### Notebook Overview

| Notebook | Description |
|--------|-------------|
| **EDA & Feature Engineering** | Data cleaning, visualization, lag features, rolling statistics |
| **Modeling – Part 1** | XGBoost, Prophet, and LSTM models |
| **Modeling – Part 2** | Transformer-based time series forecasting |

---

## Evaluation Metrics

Models are evaluated using standard regression metrics:

* **RMSE (Root Mean Squared Error)**
* **RMSPE (Root Mean Squared percentage Error)**

---

## Key Learnings

* Feature engineering is **critical** for ML-based forecasting models.
* XGBoost performs strongly when temporal features are well-designed.
* Prophet is easy to use but may underperform on complex patterns.
* LSTM and Transformer models capture temporal dependencies automatically but require:

  * More data
  * Careful training
  * Higher computational cost
