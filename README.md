# 📑 Loan Approval Prediction  

This project predicts **loan approval status** based on applicant details such as income, assets, credit score, and more.  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YourUsername/Loan-Prediction-Project/blob/main/notebook.ipynb)

---

## 📂 Dataset  
The dataset contains loan applications with the following features:  

- `loan_id`  
- `no_of_dependents`  
- `education`  
- `self_employed`  
- `income_annum`  
- `loan_amount`  
- `loan_term`  
- `cibil_score`  
- `residential_assets_value`  
- `commercial_assets_value`  
- `luxury_assets_value`  
- `bank_asset_value`  
- `loan_status` (Target: 0 = Rejected, 1 = Approved)  

---

## 🧹 Data Cleaning & Preprocessing
- Handled **missing values** and corrected data types.  
- Standardized categorical variables (`education`, `self_employed`).  
- Removed irrelevant identifiers (`loan_id`).  
- Verified distributions and unique values.  

---

## ✨ Feature Engineering
- Created **Debt-to-Income Ratio**.  
- Aggregated **Total Assets** = residential + commercial + luxury + bank assets.  
- Normalized continuous features.  

---

## 📊 Exploratory Data Analysis (EDA)
- Visualized loan approvals by **education**, **employment**, and **dependents**.  
- Analyzed relationship between **CIBIL score**, **income**, and approval rates.  
- Observed clear separability between high-score applicants and loan status.  

---

## 🔁 Train/Test Split
- **Stratified train/test split** (80/20) to maintain class balance.  
- Verified baseline distribution:  
  - Approved ≈ 62%  
  - Rejected ≈ 38%  

---

## 🤖 Models Trained
We tested multiple models for classification:  

- **Logistic Regression**  
- **Decision Tree**    
- **Tree Ensemble (Bagging)**  

---

## 📈 Results

| Model                  | Accuracy | Notes |
|-------------------------|----------|-------|
| Logistic Regression     | **0.82** | Good baseline model, interpretable |
| Decision Tree           | **0.96** | Perfect fit|
| Tree Ensemble (Bagging) | 0.9988   | Very strong |

✅ Logistic Regression gives a solid **baseline (~82% accuracy)**.  
✅ Tree-based methods achieve good accuracy.  

---

## 🛠 Tech Stack
- Python  
- Pandas / NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib / Seaborn  

---

## 🚀 Next Steps
- Test on an **unseen dataset** to confirm generalization.  
- Apply **regularization** (XGBoost params like `max_depth`, `lambda`).  
- Deploy model as an **API or web app** for real-world usage.  

---

## 🏷 License
This project is for **educational purposes**.  
