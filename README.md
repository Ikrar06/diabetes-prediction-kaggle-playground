# Diabetes Prediction - Kaggle Playground

Kaggle Playground Series Season 5 Episode 12

## Results

- **Current LB Score:** 0.70322
- **Target:** 0.706+

## Key Strategy

1. **Distribution Shift Detection**
   - Cutoff ID: 678,260 (using rolling mean analysis)
   - Last 21,740 samples match test distribution

2. **Original Dataset Features**
   - 48 features from diabetes health indicators dataset
   - Mean and count statistics for domain knowledge transfer

3. **Weighted Refit**
   - Weight = 15 on test-like samples
   - Proven improvement: +0.003 to +0.004

4. **Ensemble Methods**
   - XGBoost + LightGBM
   - Optimized weights via scipy

## Notebooks

- `cutoff_weighted.ipynb` - Main solution (LB 0.70322)
- `ultimate_0706.ipynb` - Advanced stacking approach (target 0.706+)

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Tech Stack

Python, pandas, numpy, scikit-learn, XGBoost, LightGBM
