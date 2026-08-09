# 🏡 House Price Prediction - Advanced Regression Techniques

An interactive Machine Learning project that predicts the final sale price of residential homes in Ames, Iowa, using advanced regression techniques.

✅ **Trained on the famous Ames Housing dataset**  
✅ **Extensive Feature Engineering and EDA**  
✅ **Multiple Regression ML models compared**  
✅ **Optimized for Root-Mean-Squared-Error (RMSE) on log prices**  

---

## 📌 Project Description

With 79 explanatory variables describing almost every aspect of residential homes in Ames, Iowa, this project challenges traditional predictive models to accurately estimate the final price of each home. The goal is to build a machine learning pipeline that explores the data, engineers meaningful features, and predicts the `SalePrice` variable with high precision.

- **Domain**: Real Estate Analytics / Machine Learning  
- **Target Variable**: `SalePrice` (Continuous)  
- **Features**: 79 features including physical characteristics (area, rooms, bathrooms), material quality, and temporal data (year built, year sold).

---

## 🚀 Problem Type

This is a **Supervised Regression Problem**.  
Since errors in predicting expensive houses and cheap houses should affect the result equally, we predict the **logarithm of the observed sales price** and evaluate the models using Root Mean Squared Error (RMSE).

---

## 📊 Model Comparison

| Model                 | R² Score | RMSE (Log) | Best Trait                               |
|-----------------------|----------|------------|------------------------------------------|
| Ridge Regression      | 0.8850   | 0.1350     | Handles multicollinearity, fast baseline |
| K-Nearest Neighbors   | 0.7620   | 0.1980     | Simple distance-based predictions        |
| Decision Tree         | 0.7850   | 0.1850     | Interpretable non-linear rules           |
| Random Forest         | 0.8920   | 0.1310     | Robust ensemble, stable feature bagging  |
| **XGBoost Regressor ✅**| **0.9150** | **0.1180** | **Best generalization, boosted performance** |

---

### ✅ Why XGBoost?

- ⏱️ **Efficient training** with gradient boosting.  
- 📈 **Lowest RMSE and Highest R²**, showing superior predictive accuracy.  
- 🧠 **Handles complex interactions** between the 79 variables better than linear models.  
- 🛠️ **Robust to outliers** and sparse data introduced by one-hot encoding.  

---

## 🛠️ Tech Stack

| Tool            | Use                            |
|-----------------|---------------------------------|
| Python          | Core language                  |
| Pandas / NumPy  | Data cleaning & transformation |
| Seaborn         | Visual analytics and EDA       |
| Scikit-learn    | ML models, scaling & evaluation|
| XGBoost         | Final optimized regressor      |