# 🧴 Skin Disorder Prediction Using Machine Learning

## 📌 Objective
Develop a machine learning model to predict six types of skin disorders using clinical and histopathological features. The aim is to aid early diagnosis and reduce unnecessary biopsies, supporting dermatologists in making faster, more confident decisions.

---

## 📊 Dataset Overview
- *Total Samples*: ~366
- *Total Features*: 34
  - 12 Clinical features
  - 22 Histopathological features
  - Age
- *Target Variable*: 6 disease classes

The dataset includes both visible clinical observations and histopathological test results, making it suitable for exploring early diagnostic strategies.

---

## 🛠 Data Preparation
- Verified no missing values
- Target variable properly encoded into integer class labels
- Applied stratified 80/20 train-test split to preserve class balance

---

## 🔎 Exploratory Data Analysis (EDA)
- Class imbalance observed across disease classes
- Certain features (scaling, definite borders, hyperkeratosis) showed strong separation between classes
- Heatmap analysis revealed correlations among some histopathological features
- Clinical features largely independent

---

## 🤖 Model Selection & Training
We trained and compared multiple classifiers:
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Logistic Regression
- Support Vector Machine (SVM)

✅ *Best Performing Model*: Random Forest Classifier

---

## 📈 Model Evaluation
- Random Forest achieved ~89% accuracy on the test set
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
- Random Forest delivered strong generalization and balanced performance across classes

---

## 🌟 Feature Importance Analysis
- Used Random Forest’s feature importance scores
- *Top Features*:
  - Scaling
  - Definite borders
  - Family history
  - Erythema
  - Hyperkeratosis
- Insight: Many top features are clinical, enabling early diagnosis even before biopsy.

---

## 👨‍⚕ Suggestions for Doctors
- Focus on key clinical indicators (scaling, definite borders, family history, erythema) for early screening
- Use family history and visible symptoms as early warning signs
- Machine learning can help prioritize biopsies only when necessary, improving diagnostic efficiency and reducing patient discomfort

---

## ⚙ Challenges & Solutions
- Multi-class classification addressed using Random Forest’s built-in support
- Slight class imbalance managed with stratified splitting
- Model interpretability improved via feature importance plots to aid clinical understanding

---

## ✅ Conclusion
This project demonstrates that skin disorders can be predicted with high accuracy using machine learning. Clinical features alone hold significant predictive value, supporting dermatologists in early detection and improving patient care.

---


