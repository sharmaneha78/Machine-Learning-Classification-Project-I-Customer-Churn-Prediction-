# Machine-Learning-Classification-Project-I-Customer-Churn-Prediction-
A machine learning project to predict customer churn by analyzing behavioral, demographic, and transactional data. The project includes exploratory data analysis, feature engineering, model building, performance evaluation, and actionable business insights to help companies reduce churn and improve retention strategies.
# 📌 Customer Churn Prediction – Machine Learning Project

This repository contains a complete end-to-end machine learning solution for **Customer Churn Prediction**. The goal is to identify customers who are likely to leave a service so that the company can take proactive retention actions.

---

## 🎯 Business Objective

- Predict whether a customer will churn or continue using the service.
- Analyze the factors that influence churn.
- Build a machine learning model to classify customers into churn / non-churn.
- Provide actionable business insights and recommendations to reduce churn and improve customer retention.

---

## 📁 Dataset Description

The dataset contains 19 features related to customer profile, usage patterns, revenue details, service experience, and churn status.

| Column | Description |
|--------|-------------|
| AccountID | Unique Customer ID |
| Churn | Target variable (1 = churn, 0 = not churn) |
| Tenure | Number of months customer stayed |
| City_Tier | Customer's location category |
| Payment | Mode of payment |
| Gender | Male / Female |
| Service_Score | Customer experience score |
| Account_user_count | Number of connected users |
| account_segment | Economy / Premium / Others |
| CC_Agent_Score | Support agent rating |
| complain_ly | Total complaints last year |
| rev_per_month | Monthly revenue |
| Login_device | Web / mobile |
| marital_status | Married / Single |
| feedback | Customer feedback category |
| ... | Other demographic and usage-based features |

📊 **Total Records:** 11260  
⭐ **Churn Rate Observed:** *16.8% customers are churned*

---

## 🔍 Exploratory Data Analysis Insights

| Finding | Insight |
|--------|---------|
| Tenure | New customers (low tenure) churn more |
| Complaints | High number of customer complaints strongly linked to churn |
| City Tier | Tier-3 cities show higher churn tendency |
| Payment Mode | Wallet / UPI users churn more compared to Auto-debit |
| Revenue | Low revenue users show more churn |
| Gender | Female slightly higher churn rate |
| Account Segment | Economy users churn more |

### Visual insights:
- Churn rate vs. Tenure shows steep early drop
- Revenue distribution shows clear difference between churn / non-churn groups
- Heatmap reveals strong correlations among features

---

## 🧠 Machine Learning Workflow

### Steps Followed
- Data Import & Cleaning
- Missing values handling
- Label Encoding and One-hot encoding
- Train-test split (80-20)
- Feature Scaling
- Model Training
- Model Comparison
- AUC-ROC / Confusion Matrix evaluation

### Models Built
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

---

## 📈 Model Evaluation Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | ~89% |
| Random Forest | ~94% |
| **XGBoost (Best)** | **97.46%** |

### Confusion Matrix
## [[1870 13]
## [ 44 325]]

### Classification Report
- Accuracy: 0.9746
- Precision (Churn Class): 0.96
- Recall (Churn Class): 0.88
- F1-Score: 0.92

---

## 🏆 Best Model: XGBoost Classifier

📌 Reasons for selection:
- Highest accuracy among tested models
- Best precision-recall balance
- Excellent performance on minority churn class

### Feature Importance
Most important predictors of churn:
- Tenure
- Revenue Per Month
- Complaints Last Year
- Account Segment
- Payment Method
- Service Score

---

## 🧾 Business Recommendations

| Insight | Actionable Recommendation |
|---------|---------------------------|
Low-tenure customers churn more | Create onboarding engagement & reward programs |
High complaints rate | Improve customer support response system |
Low revenue customers churn | Provide offers, bundled plans, loyalty benefits |
Wallet / UPI users churn | Encourage auto-payment with cashback |
Economy segment churn | Personalized retention campaigns |
Low service score | Improve service & monitor feedback trends |

---

## 🏁 Conclusion

- Customer churn prediction helps businesses identify at-risk customers early.
- **XGBoost achieved 97.46% accuracy**, which is suitable for production deployment.
- Key churn drivers were identified, allowing strategic decision-making.
- Implementing recommended actions can significantly reduce churn and increase revenue.

---

## 🚀 Future Scope
- Model deployment using **Flask / FastAPI**
- Integration with live dashboards
- Customer segmentation using clustering
- NLP sentiment analysis on feedback text

---
## Teck Stack
| Category        | Tools                                |
| --------------- | ------------------------------------ |
| Language        | Python                               |
| Libraries       | Pandas, NumPy, Scikit-learn, XGBoost |
| Visualization   | Matplotlib, Seaborn                  |
| IDE             | Jupyter Notebook                     |
| Version Control | Git & GitHub                         |

## 👩‍💻 Project By: Neha Sharma
Machine Learning & Data Science Enthusiast
