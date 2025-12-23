Project 1: Energy Consumption Prediction

Author: Maatla Ookeditse Mosimanyane
Date: 14 septermber 2025

Objective
The goal of this project is to predict household energy consumption using historical temperature and hour data. This can help optimize energy usage, plan loads, and improve efficiency in energy management.

Tools & Technologies
- Python 3.13 
- Pandas: For data manipulation  
- NumPy: For numerical computations  
- Matplotlib: For data visualization  
- Scikit-learn: For machine learning (Linear Regression & Random Forest Regressor)

Dataset
- Source: Generated data my me   
- Columns used:  
  - `Temperature` (°C)  
  - `Hour` (0–23)  
  - `Global_active_power` (kW) – target variable

> The dataset contains hourly energy consumption readings along with other electrical measurements.

Data Cleaning
- Removed missing values  
- Extracted hour from timestamp for modeling  
- Selected relevant columns for prediction

Machine Learning Models
1. Linear Regression
   - Simple regression to model energy based on temperature and hour
2. Random Forest Regressor
   - Ensemble model for more accurate predictions

Results
| Model                 | R² Score |
|-----------------------|----------|
| Linear Regression     | 0.95     |
| Random Forest Regressor | 0.99     |

- Example prediction:  
  - Input: Temperature = 28°C, Hour = 12  
  - Predicted Energy Consumption = 273.75 kW

Visualizations
- Scatter plots of Temperature vs Energy  
- Scatter plots of Hour vs Energy  
- Predicted vs Actual energy consumption

Applications
- Energy efficiency optimization  
- Load forecasting  
- Support for smart grid systems  

How to Run
1. Open `Energy_Consumption_Prediction.ipynb` in Jupyter Notebook  
2. Install required libraries if not already installed:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
