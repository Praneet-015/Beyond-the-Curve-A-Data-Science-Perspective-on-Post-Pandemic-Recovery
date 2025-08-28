# Beyond the Curve: A Data Science Perspective on Post-Pandemic Recovery  

This repository contains the datasets, code, figures, and report for my MSc Data Science Final Project.  
The project focuses on **forecasting COVID-19 case trends in India** and developing a **risk scoring framework** to support policymaking and post-pandemic recovery.  

---

## Project Overview  

The COVID-19 pandemic left a severe mark on India, with multiple waves of infections, overwhelmed hospitals, and major socio-economic disruption. Policymakers required reliable forecasting tools to plan healthcare capacity, track vaccination impacts, and evaluate intervention strategies.  

This project applies and compares **three forecasting models**:  
- **ARIMA** – statistical baseline  
- **Prophet** – trend and seasonality-based  
- **LSTM** – deep learning for time-series  

Additionally, the project introduces a **composite risk score** (combining case growth, vaccination coverage, and hospital demand) and a **scenario simulation** to evaluate the effects of slower vaccination rollout.  

---

## Tools and Libraries  

Implemented in **Python 3.10**, using:  
- Data handling: `pandas`, `numpy`  
- Visualisation: `matplotlib`, `seaborn`, `plotly`  
- Models: `statsmodels` (ARIMA), `prophet`, `tensorflow/keras` (LSTM)  
- Evaluation: `scikit-learn` metrics (MAE, RMSE)  
- Jupyter for analysis  

See [`requirements.txt`](requirements.txt) for full dependencies.  

---

## Repository Structure  
├── data/
│ ├── cleaned_india_covid_data.csv
│ ├── engineered_india_covid_data.csv
│ └── owid-covid-data.csv
│
├── notebooks/
│ ├── COVID_Forecasting.ipynb # main analysis
│ └── preprocessing.ipynb # cleaning & feature engineering
│
├── figures/
│ ├── descriptive/ # EDA and descriptive plots
│ ├── forecasting/ # ARIMA, Prophet, LSTM results
│ ├── risk_scores/ # risk score plots
│ └── scenarios/ # vaccination slowdown outputs
│
├── report/
│ └── Final_Project_Report.pdf # academic report
│
├── requirements.txt # dependencies
└── README.md # this file
