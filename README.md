# Retail Sales Insights & Forecasting (Aug 2023 – Oct 2023)

Analyze retail sales, explore seasonal patterns, and forecast future performance using **ARIMA** and **Prophet**.

## Key Features
- **Data Cleaning & Preprocessing**: Fill gaps, standardize daily frequency.
- **EDA**: Trend/seasonality checks (see notebooks).
- **Forecasting**: ARIMA baseline; Prophet (if available).
- **Visuals**: Matplotlib for quick plots; Tableau (optional) for dashboards.

## Project Structure
```
Retail-Sales-Forecasting/
├── data/                        # sales_data.csv (sample) & cleaned output
├── notebooks/                   # EDA & forecasting notebooks
├── outputs/                     # saved forecasts & plots
├── scripts/                     # preprocessing, models, viz
├── requirements.txt             # Python deps
├── README.md
└── LICENSE
```

## Quickstart
```bash
# 1) Create a virtual environment (recommended)
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
# source .venv/bin/activate

# 2) Install dependencies
pip install -r requirements.txt

# 3) Prepare data
python scripts/data_preprocessing.py

# 4) Run forecasts
python scripts/forecasting_models.py

# 5) Plot results (ARIMA)
python scripts/visualization.py
```

Outputs are saved under `outputs/`:
- `forecast_arima.csv`
- `forecast_prophet.csv` (if Prophet installed)
- `arima_plot.png`

## Tableau (Optional)
Export aggregated data from `data/sales_data_clean.csv` and build a KPI dashboard (Sales, 7-day MA, WoW growth).

## Tech
Python (pandas, numpy, matplotlib, statsmodels, prophet)
