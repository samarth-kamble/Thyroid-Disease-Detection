# 🧠 Thyroid Disorder Detection Using ML (KNN, SVM, Decision Tree)

This project aims to develop machine learning models to **detect thyroid disorders**, particularly **hyperthyroidism**, using clinical and demographic data. The system leverages **KNN**, **Decision Tree**, and **SVM classifiers**, integrates **SMOTE** for class balancing, and offers a user-friendly **Streamlit-based UI** for interactive predictions.

---

## 📊 Dataset Overview

- **Source**: [Kaggle - Hyperthyroid Dataset](https://www.kaggle.com/datasets)
- **Original Source**: UCI Machine Learning Repository
- **Total Records**: 9,172 patients
- **Features**: 31 attributes including:
  - **Demographic Info**: `Age`, `Sex`
  - **Medical History**: Thyroxine usage, antithyroid meds, sick, pregnant, etc.
  - **Lab Results**: `TSH`, `T3`, `TT4`, `FTI`, etc.
  - **Others**: `Referral Source`, `Patient ID`, and **Target** (Diagnosis)

> The target variable indicates the presence of **Hyperthyroidism** with multi-class labels.

---

## 🚀 Project Objective

Develop machine learning models that accurately identify patients with **hyperthyroidism** based on:

- Medical history
- Hormone levels
- Diagnostic attributes

Models are intended to support **early diagnosis** and **clinical decision-making**.

---

## ⚙️ Machine Learning Models

All models were trained using a balanced dataset via **SMOTE** to address class imbalance.

### 1. ✅ K-Nearest Neighbors (KNN)

- **Training Accuracy**: 97.63%
- **Testing Accuracy**: 95.39%
- **F1 Score**: 0.953
- **Precision**: 0.955
- **Recall**: 0.954

### 2. 🌳 Decision Tree

- **Training Accuracy**: 100%
- **Testing Accuracy**: 97.49%
- **F1 Score**: 0.975
- **Precision**: 0.975
- **Recall**: 0.975

### 3. 💻 Support Vector Classifier (SVC)

- **Training Accuracy**: 88.64%
- **Testing Accuracy**: 87.93%
- **F1 Score**: 0.878
- **Precision**: 0.880
- **Recall**: 0.879

---

## 📉 Confusion Matrix Summary

| Class | Precision | Recall | F1-Score | Support |
| ----- | --------- | ------ | -------- | ------- |
| 0     | 0.95      | 0.98   | 0.97     | 496     |
| 1     | 0.94      | 0.93   | 0.94     | 473     |
| 2     | 0.93      | 0.91   | 0.92     | 508     |

- **Overall Accuracy**: **94%**
- **Macro Avg F1-Score**: **0.94**
- **Weighted Avg F1-Score**: **0.94**

---

## 🖥️ Web App – Streamlit Interface

A clean and simple **Streamlit UI** allows users to:

- Input patient data
- Select the prediction model
- View diagnosis predictions in real-time

> Perfect for quick demo and non-technical stakeholders!

---

## 🧪 Techniques Used

- **Data Preprocessing**: Null handling, feature encoding, outlier removal
- **SMOTE**: To balance classes in training data
- **Model Evaluation**: Accuracy, Precision, Recall, F1, Confusion Matrix
- **Streamlit**: To create an interactive web interface

---

## 🛠️ Tech Stack

- **Python** (Pandas, Scikit-learn, NumPy, Matplotlib, SMOTE)
- **Streamlit** (Frontend UI)
- **Jupyter Notebook** (EDA, training, evaluation)

---

---

## 📈 Future Improvements

- Model explainability (SHAP or LIME)
- Include hypothyroidism detection
- API for mobile or web integration
- Dockerize the app

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

---

## 🙌 Acknowledgments

- [UCI ML Repository](https://archive.ics.uci.edu/)
- [Kaggle Hyperthyroid Dataset](https://www.kaggle.com/datasets)
- Scikit-learn & Streamlit communities
