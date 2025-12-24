# Diabetes Prediction - Kaggle Challenge

Playground Series Season 5 Episode 12

## Overview

Predicting diabetes diagnosis probability using clinical and demographic features.
- Metric: ROC AUC
- Target: 0.726-0.730 ROC AUC

## Project Structure

```
diabetesprediction/
├── data/                   # Dataset files
├── notebooks/              # Analysis notebooks
├── src/                    # Source code
├── submissions/            # Submission files
└── models/                 # Saved models
```

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Methodology

1. Exploratory Data Analysis
2. Feature Engineering (medical ratios, interactions)
3. Model Training (XGBoost, CatBoost)
4. Ensemble & Calibration

## Key Finding

Train-test distribution shift detected in last 22k samples. Weighted refit strategy provides significant improvement.

## Results

Work in progress.

## Technologies

Python, pandas, scikit-learn, XGBoost, CatBoost
