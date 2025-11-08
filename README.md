# ICOADS Time Series Analysis  
## Sea Surface Temperature and Marine Weather Forecasting  

**Forecasting Sea Surface Temperature (SST) and Marine Weather Variables using NOAA ICOADS Time Series Data**

---

## Project Overview

This project analyzes and forecasts **Sea Surface Temperature (SST)** and key marine weather variables—such as air temperature, wind speed, and atmospheric pressure—using NOAA’s **International Comprehensive Ocean-Atmosphere Data Set (ICOADS)**.

Using advanced forecasting models including **SARIMA**, **LSTM**, and **Prophet**, the project aims to predict future oceanic and atmospheric conditions with high precision.

---

## Motivation

The ocean drives the Earth's climate system, and accurate forecasting of SST and marine weather factors is crucial for:

- Climate monitoring and modeling  
- Marine ecosystem management  
- Maritime navigation and safety  
- Disaster risk reduction  
- Data-driven environmental insights  

---

## Dataset

**Source:** [NOAA International Comprehensive Ocean-Atmosphere Data Set (ICOADS)](https://icoads.noaa.gov/)  
**Access:** Public via [Kaggle](https://www.kaggle.com/)  
**Records:** 800M+ observations (2001 – 2017)  
**Scope Used:** 2001 – 2017 subset for computational feasibility  

**Key Variables:**
- Sea Surface Temperature (SST)  
- Air Temperature  
- Wind Speed & Direction  
- Atmospheric Pressure  
- Relative Humidity  
- Latitude / Longitude  
- Observation Time  

---

## Project Workflow

### 1. Data Aggregation
- Accessed ICOADS data using BigQuery Python Client  
- Filtered and aggregated data from 2001 – 2017  

### 2. Cleaning & EDA
- Fixed missing values and outliers  
- Performed univariate/bivariate analysis  
- Identified seasonal and spatial trends  
- Generated correlation matrices and visual summaries  

### 3. Feature Engineering
- Created time-based variables (month, year, season)  
- Added lag and rolling window features  
- Applied log transformation and differencing  
- Normalized data for model stability  

### 4. Model Development
- **SARIMA:** Baseline time series forecasting  
- **LSTM:** Multivariate, nonlinear deep learning forecasting  
- **Prophet:** Trend and seasonality-based forecasting  

### 5. Evaluation & Visualization
- Metrics: RMSE, R²  
- Visualized predicted vs actual values  
- Detected temperature anomalies and seasonal effects  
- Generated forecast projections with confidence intervals  

---

## Tools & Technologies

| Category | Tools |
|-----------|-------|
| **Language** | Python |
| **Environment** | Google Colab, Jupyter Notebooks, BigQuery Notebooks |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Modeling** | Scikit-learn, Statsmodels, PyTorch, Prophet |
| **Cloud/Data Access** | BigQuery Python Client |
| **Version Control** | Git, GitHub |

---

## Getting Started

### Requirements
```bash
python >= 3.8
pip
```

### Required Packages
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=0.24.0
statsmodels>=0.13.0
torch>=1.9.0
prophet>=1.1.0
google-cloud-bigquery>=2.26.0
jupyter>=1.0.0
```

# Project Structure
```
ICOADS-Time-Series-Analysis/
├── .github/                    # GitHub workflows
├── docs/
│   ├── plots/                  # Visualization outputs
│   └── reports/                # Final documentations
├── src/
│   ├── common/                 # Shared utilities
│   ├── data-aggregation/       # Data preprocessing
│   └── models/                 # Model implementations
├── .gitignore                  # Exclude large files
└── README.md
```

---

## Folder Overview

| Folder | Purpose |
|--------|---------|
| `.github/` | Github Config |
| `docs/plots/` | Saved visualizations & charts |
| `docs/reports/` | Final reports & analysis |
| `src/common/` | Helper functions & utilities |
| `src/data-aggregation/` | Data collection & cleaning scripts |
| `src/models/` | SARIMA, Prophet, LSTM implementations |

---

## Key Files

- **README.md** — Project overview & setup instructions
- **.gitignore** — Excludes large data files & model artifacts

## Team Members

| Member | Email | Responsibilities |
|--------|-------|------------------|
| Umaeshwer Shankar | umaeshwe@usc.edu | Data Collection, SARIMA Modeling |
| Arin Paul | arinpaul@usc.edu | Preprocessing, LSTM & Prophet Modeling |
| Alex Zhang | alexyzha@usc.edu | Exploratory Data Analysis & Feature Engineering |
| Ketan Totlani | totlani@usc.edu | Visualization & Reporting |

## Expected Outcomes

- Robust forecasting framework for SST and marine weather variables
- Identified seasonal trends and anomaly patterns
- Comparative analysis of SARIMA, LSTM, and Prophet models
- Comprehensive visualizations of model performance
- Evaluation metrics demonstrating predictive reliability
- Documented insights on correlations among oceanic and atmospheric parameters

---
