# ICOADS Time Series Analysis
# Sea Surface Temperature and Marine Weather Forecasting

Forecasting of Sea Surface Temperature and Marine Weather Variables using NOAA ICOADS Time Series Data

## 🎯 Project Overview

This project aims to analyze and forecast **Sea Surface Temperature (SST)** along with essential marine weather variables such as air temperature, wind speed, and atmospheric pressure using the NOAA International Comprehensive Ocean-Atmosphere Data Set (ICOADS). 

By leveraging advanced time series forecasting techniques including SARIMA, LSTM, and Prophet, we develop predictive models capable of estimating future oceanic and atmospheric conditions with high accuracy.

## 🌍 Motivation

Oceans play a critical role in regulating global climate. Accurate forecasting of sea surface temperature and related weather parameters is vital for:
- Climate monitoring and analysis
- Marine ecosystem management
- Navigation safety
- Disaster preparedness
- Data-driven climate analytics

## 📊 Dataset

**Source:** NOAA International Comprehensive Ocean-Atmosphere Data Set (ICOADS)

**Availability:** Publicly available through Kaggle

**Dataset Size:** Over 800 million records spanning from mid-1600s to 2017

**Project Scope:** Filtered subset from 2001 to 2017 (for computational feasibility)

**Key Variables:**
- Sea Surface Temperature (SST)
- Air Temperature
- Wind Speed and Direction
- Atmospheric Pressure
- Relative Humidity
- Latitude and Longitude
- Time of Observation

## 🔧 Project Workflow

### 1. Data Aggregation
- Access NOAA ICOADS dataset using BigQuery Python client library
- Filter for the period 2001-2017
- Aggregate marine weather data across time series

### 2. Cleaning and Exploratory Data Analysis (EDA)
- Handle missing values, outliers, and inconsistencies
- Perform univariate and bivariate analysis
- Identify seasonal trends and anomalies
- Generate correlation matrices
- Visualization: time series plots, geographical distributions
- Variable selection and grid search

### 3. Feature Engineering
- Create time-based features (month, season, year)
- Generate lag features and moving averages
- Apply log transformation and differencing
- Data scaling for improved model performance

### 4. Model Development
- **SARIMA:** Univariate baseline time series forecasting
- **LSTM:** Multivariate and nonlinear forecasting with deep learning
- **Prophet:** Seasonal forecasting with trend decomposition
- Train-test split for robust evaluation

### 5. Evaluation and Visualization
- Performance metrics: RMSE, R² Score
- Predicted vs. actual value visualizations
- Temperature trend analysis and anomaly detection
- Forecast projections and confidence intervals

## 📦 Technologies & Tools

**Programming Language:** Python

**Development Environment:** Google Colab, Jupyter Notebooks

**Data Processing:** Pandas, NumPy

**Visualization:** Matplotlib, Seaborn

**Machine Learning & Time Series:** Scikit-learn, Statsmodels, PyTorch

**Deep Learning:** LSTM via PyTorch

**Forecasting:** Prophet

**Version Control:** Git, GitHub

**Cloud/Data Access:** BigQuery Python client library

## 🚀 Getting Started

### Prerequisites
```bash
python >= 3.8
pip
```

### Installation

1. Clone the repository
```bash
git clone https://github.com/alexyzha/ICOADS-Time-Series-Analysis
cd src
```

2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages
```bash
pip install -r requirements.txt
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

# 📁 Project Structure
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
├── .gitignore
└── README.md
```

---

## 📂 Folder Overview

| Folder | Purpose |
|--------|---------|
| `.github/` | CI/CD workflows & automation |
| `docs/plots/` | Saved visualizations & charts |
| `docs/reports/` | Final reports & analysis |
| `src/common/` | Helper functions & utilities |
| `src/data-aggregation/` | Data collection & cleaning scripts |
| `src/models/` | SARIMA, Prophet, LSTM implementations |

---

## 🔑 Key Files

- **README.md** — Project overview & setup instructions
- **.gitignore** — Excludes large data files & model artifacts
- **requirements.txt** — Python dependencies

## 👥 Team Members

| Member | Email | Responsibilities |
|--------|-------|------------------|
| Umaeshwer Shankar | umaeshwe@usc.edu | Data Collection, SARIMA Modeling |
| Arin Paul | arinpaul@usc.edu | Preprocessing, LSTM & Prophet Modeling |
| Alex Zhang | alexyzha@usc.edu | Exploratory Data Analysis & Feature Engineering |
| Ketan Totlani | totlani@usc.edu | Visualization & Reporting |

## 📈 Expected Outcomes

- Robust forecasting framework for SST and marine weather variables
- Identified seasonal trends and anomaly patterns
- Comparative analysis of SARIMA, LSTM, and Prophet models
- Comprehensive visualizations of model performance
- Evaluation metrics demonstrating predictive reliability
- Documented insights on correlations among oceanic and atmospheric parameters

## 📚 References

[1] Q. Huang and Z. Cui, "Study on prediction of ocean effective wave height based on hybrid artificial intelligence model," *Ocean Engineering*, vol. 289, Part 1, p. 116137, 2023, doi: 10.1016/j.oceaneng.2023.116137.

[2] E. Popovska and G. Georgieva-Tsaneva, "Comparative Analysis of ARIMA and LSTM Models for Seasonal Times-Series Forecasting," *2024 15th National Conference with International Participation (ELECTRONICA)*, Sofia, Bulgaria, 2024, pp. 1-3, doi: 10.1109/ELECTRONICA63645.2024.11146090.

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact & Support

For questions or issues, please reach out to any of the team members listed above or open an issue on GitHub.

---

**Last Updated:** October 2025

**Project Status:** In Development