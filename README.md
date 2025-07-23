# 🧠 Personality Classification: Introvert vs Extrovert

This project uses machine learning to classify individuals as **Introverts** or **Extroverts** based on behavioral features like social activity, time spent alone, and more.

## 🔍 Problem Statement

Given data with features such as:
- Time spent alone
- Social event attendance
- Friends circle size
- Posting frequency
- Stage fear, etc.

...predict whether a person is an **Introvert** or **Extrovert**.

## 📁 Dataset

- Training & test data provided in CSV format.
- Features include both numeric and categorical values.
- Target column: `Personality` (converted to 0/1 as `Personality Encoded`).

## 🧪 Project Steps

1. **EDA (Exploratory Data Analysis)**  
   - Pair plots & joint plots
   - Visualize differences in behavior between introverts and extroverts.

2. **Preprocessing**
   - Categorical features: OneHotEncoded (Stage fear, Drained after socializing)
   - Numerical features: Imputed using median
   - StandardScaler used inside pipeline
   - ColumnTransformer to handle both types

3. **Modeling**
   - `LogisticRegression` with pipeline
   - GridSearchCV used to tune hyperparameters
   - Cross-validation for robust performance

4. **Evaluation**
   - Accuracy, F1-score, Confusion Matrix
   - Final predictions saved in a CSV file

5. **Deployment**
   - Prepared for submission or deployment with cleaned notebook and final output

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/personality-classification.git
   cd personality-classification
