# 📊 Credit Mix Classification – End-to-End Machine Learning Project

## 📌 Project Overview
Credit Mix Classification is an end-to-end machine learning project that predicts a customer’s **Credit Mix category** — **Good**, **Standard**, or **Bad** — using structured financial and behavioral data.
The project covers the complete ML lifecycle, including data cleaning, exploratory data analysis (EDA), feature engineering, outlier handling, model-specific preprocessing pipelines, and comparative evaluation of multiple ensemble models.

## 🗂️ Project Structure<br>
├── CSV_Files/<br>
│ ├── Raw and cleaned datasets used for modeling<br>
│<br>
├── images/<br>
│ ├── EDA plots, barplots, confusion matrices and so on.<br>
│<br>
├── EDA_report.html<br>
│ ├── Automated profiling report (ydata-profiling)<br>
│<br>
├── Predicting Customer Credit Mix - End-to-End.ipynb<br>
│ ├── Main notebook containing the full ML workflow<br>
│<br>
├── README.md<br>
│ ├── Project documentation

## 📁 Cleaned Dataset Description
- **Total records:** 50,000  
- **Total features:** 30
- **Target variable:** `Credit_Mix`

### Target variable --> Classes
- `Good`
- `Standard`
- `Bad`

### Feature Types
- **Numerical:** 'Age', 'Annual_Income', 'Monthly_Inhand_Salary', 'Num_Bank_Accounts', 'Num_Credit_Card', 'Interest_Rate', 'Num_of_Loan', 'Debt_Consolidation_Loan', 'Home_Equity_Loan', 'Student_Loan', 'Payday_Loan', 'Personal_Loan', 'Auto_Loan', 'Mortgage_Loan', 'Credit-Builder_Loan', 'Num_of_Loan_Types', 'Delay_from_due_date', 'Num_of_Delayed_Payment', 'Changed_Credit_Limit', 'Num_Credit_Inquiries', 'Outstanding_Debt', 'Credit_Utilization_Ratio', 'Credit_History_Months', 'Total_EMI_per_month', 'Amount_invested_monthly', 'Monthly_Balance'.
- **Categorical:** 'Occupation', 'Payment_of_Min_Amount', 'Payment_Behaviour_lavel', 'Payment_Behaviour_size'.

## 🔍 Exploratory Data Analysis (EDA)
EDA was performed using both manual visualizations and automated profiling.
📄 **EDA Report:** `EDA_report.html`

### Key Analysis Steps
- Distribution analysis
- IQR-based outlier analysis
- Feature correlation analysis
- Class imbalance inspection

## 🧹 Data Preprocessing & Feature Engineering
- Missing value handling
- Outlier detection and treatment
- Robust scaling for extreme numerical outliers
- Ordinal encoding for categorical features
- Model-specific preprocessing pipelines
- Class imbalance handling using class weights

## 🤖 Machine Learning Models
The following ensemble models were trained and evaluated:

- **Random Forest**
- **XGBoost**
- **LightGBM**

## 📈 Model Evaluation
Models were evaluated using multiple performance metrics:

- Training Accuracy
- Test Accuracy
- Precision (Weighted)
- Recall (Weighted)
- F1-Score (Weighted)
- Confusion Matrix

### 📊 Performance Summary (Test Set)

| Model         | Accuracy | F1-Score | ROC-AUC  |
|---------------|----------|----------|----------|
| Random Forest | 0.966933 | 0.966884 | 0.997442 |
| XGBoost       | 0.970933 | 0.970923 | 0.998082 |
| LightGBM      | 0.964933 | 0.964884 | 0.997703 |

## 🧠 Key Insights
- Gradient boosting models slightly outperformed Random Forest.
- RobustScaler significantly improved performance on income-related features.
- Class-weight handling effectively addressed class imbalance.

## 🛠️ Tools & Technologies
- **Programming Language:** Python  
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, XGBoost, LightGBM,
- **Visualization:** Matplotlib, Seaborn
- **EDA:** ydata-profiling

## 🚀 How to Run the Project
1. Clone the repository
2. Install required dependencies
3. Open the notebook
4. Run cells sequentially

## 👤 ---- Author ---- 
**Shahriar Hussain**  
Machine Learning & Data Science Practitioner































