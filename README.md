Kaggle Playground S5E10 – Predicting Road Accident Risk using XGBoost and LightGBM

This project predicts the likelihood of road accidents using tabular data on road, weather, and environmental conditions.  
It was created as part of the <Kaggle Playground Series – Season 5, Episode 10>.
---

## Overview
*- Goal:Predict `accident_risk` (0–1 continuous value)*
*- Algorithm: XGBoost & LightGBM*
*- Evaluation Metric: RMSE (Root Mean Squared Error)*
**- Best CV RMSE: ~0.056**

## Feature Engineering
| Feature | Description |
| `speed_curvature` | Product of speed limit × curvature |
| `lane_density` | Reported accidents per lane |
| `lighting_weather` | Combined lighting × weather condition |

## Models
1. **XGBoost Regressor** — tuned with 5-fold cross-validation  
2. **LightGBM Regressor** — identical accuracy and faster training

## Files
| File | Description |
|------|--------------|
| `road-accident-baseline-v1.ipynb` | Kaggle notebook with full workflow |
| `XGBOOSTsubmission.csv` | Final submission from XGBoost model |
| `LIGHTGBMsubmission.csv` | Final submission from LightGBM model |

## Results
- Average CV RMSE ≈ **0.056**
- Public Leaderboard: comparable to top entries in the competition  

## Links
- [Kaggle Competition] -> https://www.kaggle.com/competitions/playground-series-s5e10
- [XGBoost Docs] -> https://xgboost.readthedocs.io/
- [LightGBM Docs] -> https://lightgbm.readthedocs.io/
