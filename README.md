

Climate Change Data Analysis  

 Project Overview  
This project analyzes global climate trends using the Climate Insights Dataset. The goal is to explore key climate variables such as temperature changes, CO2 emissions, and sea level rise, and apply Linear Regression to predict temperature based on CO2 levels.  

---

Dataset Information  
- Source: Climate Insights Dataset  
- Key Variables:  
  - `CO2 Emissions` – CO2 levels in million tons  
  - `Temperature` – Global average temperature (°C)  
  - `Sea Level` – Global sea level rise (mm)  

---

Steps Taken  

1. Data Exploration & Cleaning  
Loaded and inspected dataset (`pandas`).  
Checked for missing values and handled them appropriately.  
Performed basic statistical analysis (`describe()`).  

2. Data Visualization  
Temperature Trends Over Time (`matplotlib`, `seaborn`).  
CO2 Emissions vs Temperature (scatter plot).  
Sea Level Rise Over Time.  
Heatmap of Correlations between climate variables.  

3. Machine Learning: Predicting Temperature  
Model Used: Linear Regression (`scikit-learn`).  
Feature: `CO2 Emissions`, Target: `Temperature`.  
Performance Metrics:  
   - R^2 Score: `-0.0001` (model does not explain temperature well).  
   - RMSE: `5.0747°C` (high error in predictions).  


 Model Interpretation & Findings  
- The R^2 score is very low (-0.0001), meaning CO2 alone does not strongly predict temperature.  
- The RMSE (5.0747°C) is quite high, indicating poor prediction accuracy.  
- This suggests that other factors (e.g., ocean currents, solar radiation) influence temperature more.  

How Can We Improve the Model?  
Add more features (e.g., humidity, land use changes).  
Try nonlinear models (Polynomial Regression, Decision Trees).  
Check data quality and remove any inconsistencies.  


 Files in This Repository  

`climate_analysis.ipynb` Jupyter Notebook with full analysis
`requirements.txt` List of dependencies to install
`visualizations/` Folder containing exported JPEG plots
`Climate Change Analysis Report.pdf` Summary of key findings

---

How to Run This Project  
1. Install Dependencies  
```bash
pip install -r requirements.txt
```

2. Run Jupyter Notebook  
```bash
jupyter notebook
```
Open `climate_change.ipynb` and execute the cells.

---

Conclusion  
- CO2 and temperature are related, but CO2 alone is not enough to predict temperature accurately.  
- Future improvements include adding more variables and trying different models.  
- This study aligns with climate research showing that multiple factors influence global warming.  
