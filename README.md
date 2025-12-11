# 🚢 Titanic Survival Prediction — Logistic Regression Model  
### ✔ Kodbud Data Science Internship — Task 2  
### 👤 Author: Mohammadraihan Hawaldar 

---

## 📌 Project Overview  
This project predicts whether a passenger survived the Titanic disaster using Machine Learning.  
It is developed as part of the **Kodbud Data Science Internship – Task 2: Titanic Survival Prediction**.

The goal is to build a simple yet effective **Logistic Regression model** using important passenger features such as:  
- Passenger Class (`Pclass`)  
- Sex (`Sex`)  
- Age (`Age`)  
- Number of siblings/spouses (`SibSp`)  
- Number of parents/children (`Parch`)  
- Fare (`Fare`)

---

## 📁 Dataset  
The dataset used is the official Kaggle Titanic dataset:

➡ https://www.kaggle.com/competitions/titanic/data  

The notebook automatically uses `train.csv` if uploaded.  
If not, it falls back to the seaborn Titanic dataset for demonstration.

---

## 🧹 Data Preprocessing  
The following preprocessing steps were applied:

- Imputed missing **Age** values with median  
- Filled missing **Embarked** values with mode  
- Dropped the **Cabin** column due to excessive missing data  
- Converted `Sex` to numeric (0 = male, 1 = female)  
- Created dummy variables for `Embarked`  
- Selected core predictive features:
  - `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`

---

## 🤖 Machine Learning Model  
### **Logistic Regression**  
Chosen because it is simple, effective, and perfect for binary classification tasks.

Model evaluation includes:

- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report** (precision, recall, f1-score)

---

## 📈 Results  

### **Model Accuracy:** ~80%  
A solid baseline for Logistic Regression on this dataset.

### Confusion Matrix
```
[[90 15]
 [21 53]]
```

### Highlights:
- Performs slightly better on predicting **non-survivors**
- Predicts survivors with good recall and f1-score  
- Balanced and reasonable for a baseline model

---

## 🗂 Files in This Project  

| File | Description |
|------|-------------|
| `Titanic_Kodbud_Titanic.ipynb` | Full notebook with data analysis, model training & evaluation |
| `titanic_logreg_model.joblib` | **Saved Logistic Regression model** (uploaded) |
| `titanic_scaler.joblib` | **StandardScaler used for feature preprocessing** (uploaded) |
| `train.csv` | Kaggle dataset (not stored in repo) |

---

## 🚀 How to Run  
### ✔ Recommended: Google Colab  
1. Go to https://colab.research.google.com  
2. Upload `Titanic_Kodbud_Titanic.ipynb`  
3. Upload `train.csv` from Kaggle  
4. Click **Runtime → Run all**

The notebook will:

- Preprocess data  
- Train the Logistic Regression model  
- Display evaluation metrics  
- Save model files (`.joblib`)  

---

## 🏁 Conclusion  
Through this project, the following ML skills were practiced:

- Data cleaning and preprocessing  
- Feature engineering  
- Logistic Regression modeling  
- Model evaluation  
- Data visualization  
- Saving trained models for deployment  

This project builds a strong foundation for deeper ML concepts used in real-world applications.

---

## ⭐ Author  
**Mohammadraihan Hawaldar**  
Data Science Intern @ Kodbud  
