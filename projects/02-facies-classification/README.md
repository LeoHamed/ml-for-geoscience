# Project 02: Well Log Facies Classification

## Objective
Classify lithofacies from well log data using Machine Learning.

## Dataset
- Synthetic well log data (999 samples)
- 9 faciès: Sandstone, Siltstone, Shale, Limestone, Dolomite, Coal
- Features: GR, RHOB, NPHI, DT + 4 engineered features
- Realistic missing values (6.5%) with facies-based imputation

## Models Compared
| Model | Accuracy | Best For |
|-------|----------|----------|
| Random Forest | 88.0% | Best overall after feature engineering |
| XGBoost | 87.0% | Good alternative |
| SVM | 86.5% | Strong baseline |

## Key Results
- Baseline accuracy: 84-86%
- With feature engineering: +4% improvement
- Mudstone vs Dolomite remains challenging (F1=0.67)
- Interactive Plotly visualization included

## Feature Engineering
- RHOB_NPHI_RATIO
- DENSITY_POROSITY
- GR_RHOB_PRODUCT
- NPHI_DT_PRODUCT

## Files
- `02_facies_classification.ipynb` - Full analysis

## Tools
Python, Pandas, Scikit-learn, XGBoost, Plotly, Matplotlib, Seaborn
