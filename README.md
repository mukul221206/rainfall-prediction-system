
@'
# Regime-Aware AI Post-Processing of Monsoon Rainfall Forecasts

An AI/ML-based rainfall forecasting and post-processing system that identifies synoptic weather regimes over the Indian subcontinent and applies regime-aware XGBoost bias correction to raw GFS rainfall forecasts, along with multi-threshold heavy rainfall risk classification.

## Live Demo

https://rainfall-prediction-system.vercel.app/

## System Architecture

```text
Raw GFS 0.25° NWP Forecast
            |
            v
ERA5 Atmospheric Features
(500, 700 and 850 hPa)
            |
            v
Synoptic Weather Regime Classification
            |
            v
Regime-Aware XGBoost Bias Correction
            |
            v
Corrected Rainfall Forecast
            |
            v
Heavy Rainfall Risk Classification
            |
            v
FastAPI Backend
            |
            v
React + Leaflet Dashboard