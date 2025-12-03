# 🍎 Food Freshness Predictor  
A Machine Learning project designed to predict the freshness level of food items based on environmental and storage factors such as **temperature, humidity, and storage duration**.

This project applies data preprocessing, feature engineering, and classification models—including **Random Forest** and **Gradient Boosting**—to accurately classify food as **Fresh, Stale, or Spoiled**.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Modeling Approach](#modeling-approach)
- [Results](#results)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)
- [Prediction Function](#prediction-function)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## 📝 Overview
Food spoilage is a major concern affecting food safety, public health, and economic loss.  
This project builds a **predictive system** that determines the freshness of food items based on key factors:

- Storage days  
- Ambient temperature  
- Humidity levels  
- Food category  

The model can be integrated with IoT-based refrigeration systems for **real-time spoilage detection**.

---

## 🚀 Features
- Machine learning–based food freshness classification  
- Handles **imbalanced data** using SMOTE  
- Automated **hyperparameter tuning** with GridSearchCV  
- Feature importance analysis  
- Visual insights using plots and heatmaps  
- Custom prediction function to test new inputs  

---

## 📊 Dataset
The dataset contains:

| Feature          | Description |
|------------------|-------------|
| `storage_days`   | Number of days food has been stored |
| `temperature`    | Ambient/Storage temperature |
| `humidity`       | Relative humidity level |
| `food_type`      | Category of food (Meat, Fruit, Veg, etc.) |
| `freshness`      | Target label (Fresh, Stale, Spoiled) |

Categorical features were converted using **One-Hot Encoding**.

---

## 🛠 Technologies Used
- **Python**
- **Pandas, NumPy**
- **Scikit-learn**
- **Matplotlib, Seaborn**
- **SMOTE (Imbalanced-learn)**
- **RandomForestClassifier**
- **GridSearchCV**

---

## 🤖 Modeling Approach

### ✔ 1. Data Preprocessing  
- Handling missing values  
- One-hot encoding for food types  
- SMOTE for balancing classes  

### ✔ 2. Model Training  
Algorithms used:
- **Random Forest (optimized)**
- Gradient Boosting

Random Forest was selected as the best performer after hyperparameter tuning.

### ✔ 3. Model Evaluation  
Metrics used:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## 🏆 Results

Using the tuned Random Forest model:

- **Accuracy:** 99.7%  
- High precision and recall across all classes  
- Most influential features:
  - Storage Days
  - Temperature  
  - Humidity  

---

## 📉 Visualizations

The project includes the following plots:

- **Feature Importance Bar Chart**
- **Confusion Matrix Heatmap**
- **Freshness Category Distribution Pie Chart**
- **Storage Days vs Freshness (Box Plot)**

These help interpret how environmental factors influence spoilage.

---

## ▶️ How to Run

### 1. Install dependencies
```bash
pip install numpy pandas seaborn scikit-learn imbalanced-learn matplotlib
# Food-Freshness-Predictor
