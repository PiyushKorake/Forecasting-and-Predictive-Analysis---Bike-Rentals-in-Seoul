# Forecasting and Predictive Analysis - Bike Rentals in Seoul

## Overview
This project predicts how many bikes will be rented in Seoul using past data. The goal is to help bike rental companies manage their fleet better. We tested three models – Stepwise Linear Regression, SARIMA, and XGBoost – and compared their performance to find out which works best for forecasting future demand.

## Objectives
- Understand daily and hourly bike rental trends
- Analyze patterns using EDA
- Build predictive models to estimate future demand
- Compare performance of models using RMSE, MAE, and R²
- Provide business recommendations based on the findings

## Dataset
The dataset used is **Seoul Bike Sharing Demand**, publicly available on UCI/Kaggle. It contains hourly records of bike rentals along with weather conditions and calendar info.

## Tools Used
- R programming (Tidyverse, Forecast, XGBoost packages)
- ggplot2 for visualizations
- Data pre-processing: scaling, outlier handling, feature conversion

## Models Used
1. **Stepwise Linear Regression** – helps find important features like temperature, time, and holidays.
2. **SARIMA** – captures seasonal patterns and trends over time.
3. **XGBoost** – machine learning model that gives the best prediction results.

## Key Results
| Model                    | R²     | RMSE     | MAE     |
|-------------------------|--------|----------|---------|
| Stepwise Linear         | 0.55   | 425.87   | 317.99  |
| SARIMA                  | —      | 641.49   | 512.21  |
| XGBoost                 | 0.88   | 215.43   | 122.31  |

- **XGBoost** was the most accurate and explained most of the variation in rental demand.
- Temperature, hour of the day, and whether it's a working day were the most important factors.

## Business Recommendations
- **Use XGBoost** to predict high-demand areas and allocate bikes accordingly
- **Adjust pricing** dynamically based on predicted demand
- **Plan maintenance** during low-demand hours using forecasts
- **Use seasonal trends** (from SARIMA) for better marketing and resource planning

## Future Scope
- Add weather forecasts, traffic data, and events to improve predictions
- Create real-time dashboards
- Build feedback loops to improve the model continuously

## Author
Piyush Santosh Korake  
Date: August 24, 2024
