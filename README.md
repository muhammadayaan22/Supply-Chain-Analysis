# 📦 Supply Chain Delay Prediction — Machine Learning Project

## 📌 Project Overview
This project focuses on predicting delivery delays in a supply chain system using machine learning techniques.

The goal is to determine whether an order will be delayed based on historical shipping and order data.

### 💼 Business Impact
- Improve logistics planning  
- Reduce operational costs  
- Enhance customer satisfaction  

---

## 🎯 Objective
Build a classification model to predict:

**Late Delivery Risk**
- `1` → Delayed  
- `0` → On Time  

Using features such as:
- Shipping Mode  
- Order timing (month, day, hour)  
- Product category and department  
- Shipment duration  

---

## 📊 Dataset Description

### 📌 Categorical Features:
- Shipping Mode  
- Category Name  
- Department Name  
- Order Region  

### 📌 Numerical Features:
- Days for Shipment (Scheduled)  
- Order Month / Day / Hour  

### 🎯 Target Variable:
- `Late_delivery_risk` (Binary classification)

---

## 🧹 Data Preprocessing

- ✔ Categorical Encoding: Frequency encoding applied  
- ✔ Train-Test Split: 80% training, 20% testing (stratified sampling)  
- ✔ Missing Values: Handled using mean imputation  
- ✔ Class Imbalance: SMOTE applied on training data  

---

## 🤖 Model Development

### Model Used:
- Random Forest Classifier  

### Why Random Forest?
- Handles nonlinear relationships  
- Robust to noise  
- Strong performance on tabular data  

---

## 📈 Model Evaluation

| Metric     | Score |
|------------|-------|
| Accuracy   | 68%   |
| Precision  | 73%   |
| Recall     | 72%   |
| F1-Score   | 68%   |

### 📋 Class-wise Performance

**Class 0 (On-time):**
- Precision: 0.62  
- Recall: 0.64  
- F1-score: 0.63  

**Class 1 (Delayed):**
- Precision: 0.73  
- Recall: 0.72  
- F1-score: 0.72  

---

## 📊 Key Insights

- The model performs better at predicting delayed orders  
- Slight bias toward Class 1 (Delayed)  
- Frequency encoding reduced categorical richness  
- SMOTE improved balance but introduced synthetic noise  

---

## ⚠️ Limitations

- Moderate accuracy (68%)  
- Basic feature engineering  
- No hyperparameter tuning applied  
- Frequency encoding may reduce category interpretability  
- Limited optimization of model performance  

---

## 🚀 Recommendations for Improvement

### 🔹 Feature Engineering
- Delay ratio (actual vs scheduled shipping)  
- Weekend vs weekday indicator  
- Peak hour detection  

### 🔹 Encoding Techniques
- One-hot encoding  
- Target encoding  

### 🔹 Model Improvements
- XGBoost  
- Gradient Boosting  

### 🔹 Optimization
- Hyperparameter tuning (depth, estimators, splits)  

### 🔹 Evaluation Focus
- Improve Recall and F1-score  

---

## 🧠 Conclusion

This project demonstrates an end-to-end machine learning pipeline for supply chain delay prediction.

### Key Outcomes:
- Built a working predictive model  
- Identified key delay patterns in operations  
- Demonstrated the importance of feature engineering  

### 💡 Final Insight:
Delivery delays are predictable using historical data, but feature engineering plays a more critical role than model complexity.

---

## 📌 Future Work
- Deploy model using Streamlit / Flask  
- Build real-time prediction system  
- Use ensemble methods (Stacking, Boosting)  
- Integrate external factors (weather, traffic, holidays)  

---

## 🏁 Final Note
This project follows a complete data science workflow:

**Data → Preprocessing → Feature Engineering → Modeling → Evaluation → Insights**

It demonstrates strong skills in:
- Data Analysis  
- Machine Learning  
- Business Problem Solving  
