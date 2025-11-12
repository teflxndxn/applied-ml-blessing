# Project 04
# Project 04: Predicting a Continuous Target (Titanic)

**Objective:** Predict passenger **fare** from features such as age, family size, class, sex, and embarkation port.

**Methods:** Linear Regression, Ridge, Elastic Net, Polynomial (degree 3 & 5).  
**Best model:** Ridge (Test R² ≈ 0.45, lower RMSE/MAE than baseline Linear).  
**Notes:** Polynomial fits did not outperform regularized linear models; fares are skewed with outliers.

- 📓 Full notebook: [View on GitHub](https://github.com/teflxndxn/applied-ml-blessing/blob/main/notebooks/project04/ml04_blessing.ipynb)
 
- 📁 Source folder: `notebooks/project04/`

## Results Summary (Test)
| Model | R² | RMSE | MAE |
|---|---:|---:|---:|
| Ridge (α=1.0) | 0.453 | 28.13 | 17.87 |
| Linear | 0.447 | 28.28 | 17.99 |
| ElasticNet (α=0.3, l1_ratio=0.5) | 0.406 | 29.32 | 17.62 |
| Polynomial (d=3) | 0.370 | 30.18 | 15.03 |

## Plots
- Polynomial Regression (degree 3): Age vs Fare  
- Polynomial Regression (degree 5): Age vs Fare
