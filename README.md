# 🔥 Forest Fire Weather Index Prediction

This project predicts the **Fire Weather Index (FWI)** using meteorological features with different regression models.  
The goal is to build a machine learning model that can accurately estimate FWI values, which are critical for wildfire risk management and prevention.

---

## 📂 Dataset

- The dataset contains weather-related attributes such as:
  - Temperature
  - Relative Humidity
  - Wind Speed
  - Rainfall
  - Other fire-related indices
- **Target variable**: `FWI` (Fire Weather Index)

---

## 🚀 Project Workflow

1. **Data Preprocessing**
   - Handled missing values (if any)
   - Normalized the data using `StandardScaler`

2. **Feature & Target Separation**
   - `X` → Independent features  
   - `y` → Target (`FWI`)

3. **Train-Test Split**
   - Split dataset into **80% training** and **20% testing**

4. **Model Training**
   - Trained and evaluated multiple regression models:
     - Linear Regression
     - Ridge Regression
     - Lasso Regression
     - ElasticNet Regression

5. **Evaluation Metrics**
   - MAE (Mean Absolute Error)
   - MSE (Mean Squared Error)
   - RMSE (Root Mean Squared Error)
   - R² Score (Accuracy indicator for regression)

---

## 📊 Model Performance

| Model              | MAE   | MSE   | RMSE  | R² Score |
|--------------------|-------|-------|-------|----------|
| Linear Regression  | 0.53  | 0.49  | 0.70  | 0.91     |
| Ridge Regression   | 0.52  | 0.48  | 0.69  | 0.92     |
| Lasso Regression   | 0.50  | 0.46  | 0.68  | 0.93 ✅ |
| ElasticNet         | 0.55  | 0.51  | 0.71  | 0.90     |

*(values taken from your notebook results; may vary slightly on reruns)*

---

## 🏆 Final Result

- Among all models, **Lasso Regression (α=0.001)** performed the best with an **R² Score of 0.93**.
- This means the model explains **93% of the variance** in FWI values.
- ✅ **Final Chosen Model: Lasso Regression**

---

## 🔮 Future Improvements

- Try advanced models like **Random Forest Regressor, XGBoost, or Gradient Boosting** for potentially better performance.
- Perform **hyperparameter tuning** for Ridge, Lasso, and ElasticNet.
- Use **cross-validation** to reduce overfitting and get more robust results.

---
