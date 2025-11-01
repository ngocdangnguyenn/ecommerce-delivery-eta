# E-commerce Delivery Time Prediction

Practical machine learning project predicting food delivery times with **Linear Regression achieving 82.4% R² accuracy**. Simple model with quality feature engineering outperforms complex algorithms, predicting delivery times within ±9 minutes for operational planning.

## Overview

This project uses a Food Delivery Times Dataset (Kaggle) and focuses on simple, effective regression models. The pipeline ingests raw operational features (distance, weather, traffic, courier experience), handles missing values systematically, and produces trained models ready for deployment. Key improvements include explainable feature engineering with interaction terms and careful train/test handling to avoid leakage.

The final model demonstrates that Linear Regression with quality feature engineering achieves excellent predictive performance with strong business interpretability - proving that simplicity often beats complexity.

## Quick Start

```bash
git clone https://github.com/ngocdangnguyenn/ecommerce-delivery-eta.git
cd ecommerce-delivery-eta
pip install -r requirements.txt
jupyter notebook notebooks/
```

## Project Structure

```
├── data/
│   ├── raw/
│   │   └── Food_Delivery_Times.csv    
│   └── processed/                      
│       ├── processed_data.csv          
│       ├── X_engineered.csv            
│       ├── y_target.csv               
│       ├── X_train.csv, X_test.csv    
│       └── y_train.csv, y_test.csv    
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb    
│   ├── 02_data_preprocessing.ipynb            
│   ├── 03_feature_engineering.ipynb          
│   └── 04_model_training.ipynb              
├── models/
│   └── best_model_linear_regression.pkl     
├── requirements.txt                          
└── README.md
```

## Key Results

- **Best Model**: Linear Regression (simple and effective)
- **Performance**: R² = 82.4% (RMSE = 8.89 minutes, MAE = 6.12 minutes) 
- **Key Predictors**: Distance_km (0.78 correlation), Distance×Experience interaction
- **Philosophy**: Simple models with quality features > Complex algorithms

## Model Performance Comparison
| Model | R² Score | RMSE (min) | MAE (min) |
|-------|----------|------------|-----------|
| **Linear Regression** | **0.824** | **8.89** | **6.12** |
| Ridge Regression | 0.823 | 8.89 | 6.13 |
| Lasso | 0.766 | 10.23 | 7.18 |

## Contact
- **Email**: nndnguyen2016@gmail.com
- **LinkedIn**: https://www.linkedin.com/in/ngocdangnguyenn  
- **Portfolio**: https://ngocdangnguyenn.github.io/portfolio/