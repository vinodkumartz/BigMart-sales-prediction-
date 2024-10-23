

# BigMart Sales Data Analysis and Prediction 🛒📊

This project involves building machine learning models to analyze and predict sales for **BigMart** based on historical sales data. The goal is to gain insights from the data and develop models that can accurately forecast future sales for different stores and products.

---

## Table of Contents
1. [Overview](#overview)  
2. [Dataset](#dataset)  
3. [Project Pipeline](#project-pipeline)  
4. [Models Used](#models-used)  
5. [Results](#results)  
6. [Dependencies](#dependencies)  
7. [How to Run](#how-to-run)  
8. [Conclusion and Future Work](#conclusion-and-future-work)  

---

## Overview
BigMart, a major retail chain, aims to leverage its data to forecast future sales for improved planning and inventory management. This project applies machine learning techniques to predict sales, providing actionable insights to enhance business operations.

---

## Dataset
- **Dataset Size:** 8,523 rows and 12 columns  
- **Target Variable:** `Item_Outlet_Sales` (Sales amount for each product)  
- **Key Features:**  
  - `Item_Identifier`: Unique product ID  
  - `Outlet_Identifier`: Store ID  
  - `Item_Weight`, `Item_Visibility`, `Item_Type`: Product-related attributes  
  - `Outlet_Size`, `Outlet_Location_Type`, `Outlet_Type`: Store-related attributes  

---

## Project Pipeline
1. **Data Preprocessing:**  
   - Handled missing values (e.g., imputed `Item_Weight` values).  
   - Transformed categorical features using label encoding and one-hot encoding.  
   - Scaled numerical features to normalize values.  

2. **Exploratory Data Analysis (EDA):**  
   - Analyzed sales trends based on product type, store type, and store location.  
   - Visualized relationships between product visibility, weight, and sales using scatter plots and heatmaps.  

3. **Feature Engineering:**  
   - Created new features (e.g., `Item_Fat_Content` grouped into fewer categories).  
   - Derived interaction variables such as product visibility per outlet type.  

---

## Models Used
- **Linear Regression:** Baseline model for sales prediction  
- **Random Forest Regressor:** Handled non-linearity and interactions well  
- **XGBoost:** Tuned hyperparameters for better accuracy  
- **Support Vector Machine (SVM):** Tried for comparison, though less effective  

---

## Results
- **Best Model:** Random Forest Regressor  
- **R² Score:** 93.75% (on training data)  
- **Test Accuracy:** 55.26%  
- **Mean Squared Error (MSE):** Lowest with the Random Forest model  

The **Random Forest** model performed best, balancing complexity and accuracy, and generalizing well to unseen data.  

---

## Dependencies
- Python 3.x  
- Libraries:  
  - **pandas**: Data manipulation  
  - **numpy**: Numerical operations  
  - **scikit-learn**: Machine learning models  
  - **matplotlib** and **seaborn**: Data visualization  
  - **XGBoost**: Gradient boosting  

---

## How to Run
1. Clone the repository:  
   ```bash
   git clone <repository-url>
   ```  
2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  
3. Open and run the Jupyter notebook:  
   ```bash
   jupyter notebook BigMart_Sales_Data_Analysis_and_Prediction_💰.ipynb
   ```  

---

## Conclusion and Future Work
This project demonstrates the potential of machine learning in retail sales prediction. By analyzing sales patterns and building predictive models, retailers like BigMart can improve decision-making and inventory planning.

**Future Improvements:**  
- Try advanced models like LightGBM or CatBoost for higher accuracy.  
- Perform hyperparameter tuning for further optimization.  
- Use time-series forecasting methods to capture temporal trends.

