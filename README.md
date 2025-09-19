# 🩺 Diabetes Prediction using Logistic Regression

This repository contains an implementation of **Logistic Regression** to predict diabetes using the **Pima Indians Diabetes Dataset**.  
It demonstrates an end-to-end data science workflow: data preprocessing, exploratory analysis, feature scaling, model training, evaluation, and interpretation.

---

## 📂 Repository Structure

```
├── diabetes.csv                  # Dataset (Pima Indians Diabetes)
├── APR_assignment-1.ipynb        # Jupyter Notebook with full implementation
├── README.md                     # Project documentation
```

---

## 📊 Dataset

- **Name:** Pima Indians Diabetes Dataset  
- **Source:** Kaggle / UCI Machine Learning Repository  
- **Description:** Medical diagnostic dataset used to predict whether a patient has diabetes based on features like:
  - Pregnancies
  - Glucose
  - Blood Pressure
  - Skin Thickness
  - Insulin
  - BMI
  - Diabetes Pedigree Function
  - Age  

Target variable:  
- `1` → Diabetes  
- `0` → No Diabetes  

---

## ⚙️ Steps Implemented in Notebook

1. **Data Loading & Exploration**
   - Checked shape, dtypes, summary statistics, and class balance.

2. **Missing Value Treatment**
   - Replaced invalid zeros in features (`Glucose`, `BloodPressure`, `BMI`, etc.) with `NaN`.
   - Imputed missing values with median.

3. **Exploratory Data Analysis (EDA)**
   - Target distribution plots, correlation heatmaps.

4. **Data Preprocessing**
   - Feature scaling using `StandardScaler`.

5. **Train-Test Split**
   - 80% training, 20% testing.

6. **Model Training**
   - Logistic Regression with `class_weight='balanced'`.

7. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1-score, ROC-AUC.

8. **Visualization**
   - Confusion matrix, ROC curve, Feature correlation.

9. **Feature Importance**
   - Interpreted coefficients.

---

## 📈 Results

- **Baseline Logistic Regression Accuracy:** ~77%  
- **ROC-AUC Score:** ~0.81  
- **Insights:**  
  - Glucose, BMI, and Age are strong predictors.  
  - Recall is more important in medical predictions to minimize false negatives.  

---

## 🛠️ Usage

### Clone Repository
```bash
git clone hhttps://github.com/koppolu-buddha-bhavan/APR_Assignment-1.git
cd APR_Assignment-1
```

### Open Jupyter Notebook
```bash
jupyter notebook APR_assignment-1.ipynb
```

---

## 📦 Requirements

- Python 3.8+  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  
- imbalanced-learn  

