# Epic Coffee Model (ECM)
A research framework for forecasting coffee prices using weather data, fundamentals, and machine learning.  
The project starts with Brazil and is designed to extend to Vietnam, Colombia, and eventually other commodities.

## Objectives
- Build a reusable data pipeline for market, weather, flow, and fundamental data.
- Analyze relationships across different time scales, including lag effects and non-linear patterns.
- Use weather forecasts combined with historical relationships to estimate supply/price impacts.
- Train models to forecast 5-day, 10-day, and 30-day price moves (regressions + GBM).

## Project Structure (initial)
```
epic-coffee-model/
│
├── src/
│   ├── data_ingestion/
│   │   ├── weather/
│   │   │   ├── fetch_historic.py
│   │   │   ├── fetch_forecast.py
│   │   │   ├── utils_weather.py
│   │   ├── market/
│   │   └── ...
│   │
│   ├── features/
│   ├── models/
│   ├── analysis/
│   └── config/
│       ├── api_keys.json
│       ├── regions.json     
│       └── params_weather.json
│
├── notebooks/
│   ├── 01_exploration_weather.ipynb
│   ├── 02_cleaning_weather.ipynb
│   └── 03_feature_checks.ipynb
│
├── data/
│   ├── raw/
│   │   ├── weather/
│   │   ├── market/
│   └── processed/
│
├── tests/
├── README.md
├── .env
└── requirements.txt
```
## Status
Early setup stage. Environment and data pipeline will be added next.
