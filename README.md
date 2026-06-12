# 🔄 Customer Churn Prediction

A machine learning project to predict whether a customer will churn (leave) using scikit-learn. Built with a full pipeline: EDA → preprocessing → model training → evaluation → deployment-ready inference.

---

## 📁 Project Structure

```
customer-churn-prediction/
│
├── data/
│   └── churn_data.csv          # Sample dataset (Telco-style)
│
├── notebooks/
│   └── eda_and_modeling.ipynb  # Exploratory Data Analysis + modeling walkthrough
│
├── src/
│   ├── preprocess.py           # Data cleaning & feature engineering
│   ├── train.py                # Model training & saving
│   ├── evaluate.py             # Metrics, confusion matrix, ROC curve
│   └── predict.py              # Inference on new data
│
├── models/
│   └── churn_model.pkl         # Saved trained model (generated after training)
│
├── reports/
│   └── classification_report.txt  # Output metrics (generated after evaluation)
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 🚀 Quick Start

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Train the model
```bash
python src/train.py
```

### 4. Evaluate the model
```bash
python src/evaluate.py
```

### 5. Predict on new data
```bash
python src/predict.py
```

---

## 📊 Dataset

Uses a synthetic Telco-style dataset with features like:
- `tenure` — months as a customer
- `MonthlyCharges` — monthly bill amount
- `TotalCharges` — total amount billed
- `Contract` — month-to-month, one year, two year
- `InternetService`, `TechSupport`, `OnlineSecurity`, etc.
- `Churn` — target variable (Yes/No)

---

## 🤖 Models Used

| Model | Accuracy |
|---|---|
| Logistic Regression | ~80% |
| Random Forest | ~85% |
| Gradient Boosting | ~86% |

Best model is saved to `models/churn_model.pkl`.

---

## 📈 Evaluation Metrics

- Accuracy, Precision, Recall, F1-Score
- ROC-AUC Score
- Confusion Matrix
- Feature Importance Plot

---

## 🛠️ Tech Stack

- Python 3.8+
- scikit-learn
- pandas, numpy
- matplotlib, seaborn
- joblib

---

## 📄 License

MIT License
