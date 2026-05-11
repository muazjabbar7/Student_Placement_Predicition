# 🎓 Student Placement Prediction

## 📌 Project Overview
This project predicts whether a college student will get placed based on academic and extracurricular features. Built with **Python** and **scikit-learn**, it compares multiple classification algorithms to identify the best model for placement prediction.

## 📊 Dataset
- **Size**: 10,000 student records
- **Features**: IQ, CGPA, Previous Semester Result, Academic Performance, Internship Experience, Extra-Curricular Score, Communication Skills, Projects Completed
- **Target**: Placement (Yes/No)
- **Note**: Imbalanced dataset (83% Not Placed, 17% Placed)

## 🔍 Key Steps

### 1. Exploratory Data Analysis
- Distribution analysis with histograms and QQ plots
- Correlation heatmaps and boxplots for outlier detection
- Count plots showing placement vs internship experience

### 2. Preprocessing
- **ColumnTransformer** with:
  - `MinMaxScaler` for numeric features (CGPA, IQ, scores)
  - `OneHotEncoder` for categorical feature (Internship Experience)
- **Outlier treatment**: Winsorization (capping at 1st and 99th percentiles) for IQ column
- **Class imbalance handling**: `class_weight='balanced'` in all models

### 3. Models Tested
| Model | Accuracy |
|-------|----------|
| Decision Tree | **97.87%** |
| Random Forest | 97.09% |
| Logistic Regression | 83.55% |

### 4. Evaluation Metrics
- Accuracy, Precision, Recall, F1-Score
- 5-fold Cross-Validation
- Classification Report

Author
Muazjabbar  email: muazjabbar7@gmail.com
