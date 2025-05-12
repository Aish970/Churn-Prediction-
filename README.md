# 📉 Customer Churn Prediction

## 📌 Overview
Customer churn — when users stop using a company’s product or service — presents a major risk to business revenue and growth. This project aims to **predict churn behavior** using various machine learning models, enabling proactive customer retention strategies.

## 👥 Team Members
- Aishwarya Bhethanabotla  
- Samiksha Sunil Dhemse  
- Hemant Pillala  
- Neelaveni Ushakela  

## 🧠 Methodology

### 🔍 Problem Statement
Understanding customer churn is critical to minimizing losses and improving user retention. We analyze customer usage and profile data to identify churn predictors and classify customers accordingly.

### 📊 Dataset Features
- **Call Failure**: Number of failed calls  
- **Complains**: Whether the customer has filed complaints  
- **Subscription Length**: Duration of subscription  
- **Charge Amount**: Total charge amount  
- **Seconds of Use / Frequency of Use / Frequency of SMS**  
- **Distinct Called Numbers / Age Group / Tariff Plan / Status / Age**  
- **Customer Value / FN / FP**  
- **Churn** (Target): 1 = churned, 0 = retained

## ⚙️ Data Preprocessing
- **Dropped Redundant Features**: `Charge Amount`, `Frequency of SMS`  
- **Dropped Irrelevant Features**: `Age`, `Subscription Length`  
- **Log Transform**: Applied to `Customer Value`  
- **Interaction Features**: 
  - `Customer_Value_Complains` = Customer Value × Complains  
  - `Usage_Intensity` = Frequency of Use ÷ Seconds of Use  
- **One-Hot Encoding**: For categorical columns (`Tariff Plan`, `Age Group`)  
- **Scaling**: StandardScaler applied  
- **Class Imbalance**: Addressed with SMOTE after train-test split  

## 🤖 Models Trained
- **Logistic Regression**  
- **Decision Tree**  
- **Random Forest**  
- **XGBoost**  
- **Naive Bayes**  
- **K-Nearest Neighbors (KNN)**  
- **Support Vector Machine (SVM)**  
- **Artificial Neural Network (ANN)**  
- **Gradient Boosting**  
- **AdaBoost**

## 🏆 Best Performing Models
- **🏅 Random Forest**: Highest accuracy and ROC-AUC  
- **🥈 XGBoost**: Strong performance with high recall  
- **🏋️ ANN**: Strong in capturing feature interactions  
- Simpler models like **Logistic Regression** and **Naive Bayes** served as baselines

## 📈 Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  
- Confusion Matrices and Performance Plots  

## 📌 Conclusion
Random Forest emerged as the top-performing model, followed by XGBoost and ANN. Future improvements include more refined hyperparameter tuning, advanced feature engineering, and expanded evaluation on real-time datasets.

## 📎 Dependencies
- Python 3.x  
- scikit-learn  
- XGBoost  
- pandas  
- numpy  
- matplotlib / seaborn  
- imbalanced-learn  

## ✅ To Run
1. Clone this repo  
2. Install dependencies  
3. Run `main.py` or the corresponding notebook to see training and evaluation outputs

---

Feel free to fork, explore, and enhance the model. ⭐
