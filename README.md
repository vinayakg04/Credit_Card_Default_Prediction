# 🧠 Credit Card Default Prediction using Machine Learning

Predicting whether a customer will default on their credit card payment is a crucial task in credit risk management. This project leverages Machine Learning algorithms to classify credit card customers based on their likelihood to default in the upcoming month, helping financial institutions reduce risk and make better lending decisions.

![ML Banner](https://img.freepik.com/premium-vector/machine-learning-banner-artificial-intelligence-big-data-analysis-technology-business-internet-concept-futuristic-background-illustration_67349-1544.jpg)

![UI Image](https://github.com/vinayakg04/Credit_Card_Default_Prediction/blob/master/docs/snip1.PNG)

---

## 🚀 Project Highlights

- 🔍 **Problem Statement**: Classify customers who are likely to default on their credit card payment next month.
- 🧰 **Tech Stack**: Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost
- 📊 **Algorithms Used**: Logistic Regression, Random Forest, XGBoost, SVM, KNN
- 📈 **Evaluation Metrics**: Accuracy, F1-Score, Precision, Recall, ROC-AUC
- 🎯 **Goal**: Build an interpretable, high-performing classification model to assist financial decision-makers.

---

## 📁 Dataset

- **Source**: UCI Machine Learning Repository
- **Records**: 30,000+
- **Features**: 23
- **Target Variable**: `default.payment.next.month` (0 = No Default, 1 = Default)
- **Fields Include**:
  - Credit Limit, Gender, Education, Marital Status
  - Payment History (last 6 months)
  - Bill Statement & Payment Amounts

---

## 🧪 Workflow

1. **Data Cleaning**  
   - Handle missing/null values  
   - Fix inconsistent category labels  
   - Remove outliers (Z-score, IQR methods)

2. **Exploratory Data Analysis (EDA)**  
   - Class imbalance visualization  
   - Correlation heatmap  
   - Distribution of features (e.g., Education, Age)

3. **Feature Engineering**  
   - Label Encoding  
   - Payment ratio & bill utilization metrics  
   - One-hot encoding for categorical features

4. **Model Training & Tuning**  
   - Train-test split (80:20)  
   - GridSearchCV for hyperparameter tuning  
   - Cross-validation to ensure generalization

5. **Evaluation**  
   - Confusion Matrix  
   - ROC-AUC Curve  
   - Feature Importance Ranking

6. **Deployment (Optional)**  
   - Streamlit UI for live prediction  
   - Flask API for backend integration

---

## 📊 Results

| Model              | Accuracy | F1 Score | ROC-AUC |
|-------------------|----------|----------|---------|
| Logistic Regression | 80.6%   | 0.57     | 0.76    |
| Random Forest       | 84.3%   | 0.62     | 0.82    |
| XGBoost             | **85.7%**   | **0.65**     | **0.85**    |
| SVM                 | 81.2%   | 0.59     | 0.77    |

✅ **XGBoost outperformed all other models in terms of accuracy and AUC score.**

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/credit-card-default-prediction.git
cd credit-card-default-prediction
pip install -r requirements.txt
