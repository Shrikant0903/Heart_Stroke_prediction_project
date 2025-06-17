# Heart_Stroke_prediction_project
# 🧠 Heart Stroke Prediction System

This project aims to predict the likelihood of a person having a stroke using patient data. It uses machine learning models built with **Pandas**, **Numpy**, **Seaborn**, and **Scikit-learn** to analyze health factors and provide accurate predictions.

---

## 📁 Dataset Source

The dataset is taken from [Kaggle – Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset) and includes features like:

- Gender, Age, Hypertension, Heart Disease
- Ever Married, Work Type, Residence Type
- Average Glucose Level, BMI, Smoking Status
- Target Variable: `stroke` (1 = stroke, 0 = no stroke)

---

## 🔧 Technologies Used

- Python 🐍  
- Pandas 📊  
- Numpy 🔢  
- Seaborn & Matplotlib 📈  
- Scikit-learn 🤖  

---

## ⚙️ ML Algorithms Used

- ✅ Logistic Regression  
- ✅ Decision Tree Classifier  
- ✅ Random Forest Classifier  

---

## 📊 Model Performance Summary

| Model              | Accuracy | Stroke Recall | Stroke Precision | Notes |
|-------------------|----------|----------------|-------------------|-------|
| Logistic Regression | 93.9%   | 0.00           | 0.00              | Misses stroke cases entirely |
| Decision Tree       | 91.3%   | 18%            | 23%               | Slight improvement |
| Random Forest       | 93.9%   | 0.00           | 0.00              | Still fails on minority class |

---

## ⚠️ Challenges Faced

- **Imbalanced Dataset:** Most entries are `non-stroke`, so models tend to predict only the majority class.
- **Low Recall on Stroke Class:** Models often miss stroke predictions even if accuracy is high.

---

## 💡 Future Improvements

To improve prediction on stroke cases (minority class):

- ✅ Use **SMOTE** or **ADASYN** for balancing
- ✅ Use `class_weight='balanced'` in ML models
- ✅ Explore **XGBoost**, **LightGBM** for better results
- ✅ Perform **GridSearchCV** for hyperparameter tuning
- ✅ Focus on **Recall**, **Precision**, **F1-score** rather than just accuracy

---

## 📌 Real-World Importance

> In medical diagnosis, **false negatives are dangerous**. This system focuses on minimizing missed stroke predictions, aiming for **high recall** to catch stroke risks early.

---

## 📷 Output Visualization

- 📈 Correlation heatmap  
- 🔍 Feature importance from Random Forest  
- 📊 Confusion Matrix for each model  
- 📉 Class distribution plots  

(Generated in the notebook.)

---

## 🧪 How to Run

1. Clone the repo  
   ```bash
   git clone https://github.com/Shrikant0903/Heart_Stroke_Prediction.git
   cd Heart_Stroke_Prediction
