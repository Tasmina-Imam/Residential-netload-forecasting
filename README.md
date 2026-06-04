# Residential Net-Load Forecasting Using Statistical and Learning-Based Models

## Overview

The increasing adoption of behind-the-meter (BTM) solar photovoltaic systems has introduced significant variability and uncertainty into residential power systems. Accurate net-load forecasting is essential for reliable grid operation, demand management, renewable energy integration, and energy market participation.

This project presents a comprehensive comparative study of statistical, machine learning, and deep learning approaches for day-ahead residential net-load forecasting. All models were evaluated under a unified experimental framework using identical datasets, preprocessing procedures, feature engineering techniques, and evaluation metrics to ensure a fair comparison.



## Research Objectives

- Develop accurate day-ahead residential net-load forecasting models.
- Compare classical statistical models with modern learning-based approaches.
- Evaluate both deterministic and probabilistic forecasting performance.
- Investigate the impact of feature engineering on model accuracy.
- Assess model robustness under different historical training-window lengths.

---

## Dataset

### Source

- Pecan Street Dataport
- Residential customers in Austin, Texas, USA

### Data Components

- Residential electricity consumption
- Behind-the-meter solar generation
- Historical weather measurements

### Weather Variables

- Cloud Cover
- Apparent Temperature
- Surface Pressure
- Rainfall
- Direct Radiation
- Direct Normal Irradiance (DNI)
- Direct Radiation Instantaneous



## Forecasting Models

### Statistical Models

- ARIMAX (AutoRegressive Integrated Moving Average with Exogenous Variables)
- SARIMAX (Seasonal ARIMAX)

### Machine Learning Models

- Gradient Boosting Regressor (GBR)

### Deep Learning Models

- Temporal Fusion Transformer (TFT)



## Feature Engineering

The following engineered features were incorporated:

### Temporal Features

- Hour of Day (sin/cos encoding)
- Day of Week (sin/cos encoding)
- Month (sin/cos encoding)
- Weekend Indicator
- Daytime Indicator

### Lagged Features

- Historical Net Load Lags
- Historical Weather Lags
- Daily and Weekly Seasonal Patterns

Feature engineering was found to significantly improve forecasting performance, particularly for learning-based models.


## Evaluation Metrics

### Deterministic Metrics

- Mean Absolute Error (MAE)
- Root Mean Square Error (RMSE)
- Normalized RMSE (NRMSE)
- Coefficient of Determination (R²)

### Probabilistic Metrics

- Continuous Ranked Probability Score (CRPS)
- Pinball Loss
- Prediction Interval Coverage Probability (PICP)
- Prediction Interval Width (PIW)


## Results

### Best Performing Model

**Temporal Fusion Transformer (TFT) with Feature Engineering**

| Metric | Value |
|----------|----------|
| R² | 0.923 |
| RMSE | 5.56 |
| CRPS | 2.99 |

### Key Findings

- Deep learning models achieved the highest forecasting accuracy.
- Feature engineering contributed significantly to performance improvements.
- TFT consistently outperformed statistical and machine learning models.
- Model rankings remained stable across varying training-window lengths.
- Probabilistic forecasts provided valuable uncertainty quantification for grid operations.


## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Statsmodels
- PyTorch
- PyTorch Forecasting
- Lightning

---

## Repository Structure

```text
├── data/
├── notebooks/
├── models/
├── results/
├── figures/
├── src/
├── README.md
```

---

## Applications

This work has direct applications in:

- Smart Grid Operations
- Renewable Energy Integration
- Demand Response Programs
- Distribution System Planning
- Energy Management Systems
- Grid Reliability Enhancement

---

## Thesis Information

**Master of Engineering Science (Electrical Engineering)**

Lamar University

Research Area:
Power Systems • Renewable Energy • Machine Learning • Forecasting Analytics

---

## Author

**Tasmina Imam**

Electrical Engineer | Power Systems | Renewable Energy | Machine Learning | Data Analytics

LinkedIn: www.linkedin.com/in/tasmina-imam

GitHub: github.com/Tasmina-Imam
