# 🏦 Loan Prediction Analysis & Classification
---
## 📌 Project Overview
Predicting loan eligibility is a core task for financial institutions. This project involves building a machine learning model to automate the process of identifying whether a customer is eligible for a loan based on their profile. By analyzing variables such as credit history, income, and education, the model provides a data-driven approach to risk assessment.

---

## 📂 Dataset Details
The dataset consists of various applicant attributes used to determine loan approval status.

### Key Features
| Feature | Description |
| :--- | :--- |
| **Loan_ID** | Unique identifier for each loan application |
| **Gender** | Male / Female |
| **Married** | Marital status of the applicant |
| **Dependents** | Number of people dependent on the applicant |
| **Education** | Graduate / Under Graduate |
| **Self_Employed** | Whether the applicant is self-employed |
| **ApplicantIncome** | Primary applicant's income |
| **CoapplicantIncome** | Co-applicant's income |
| **LoanAmount** | Total loan amount requested |
| **Loan_Amount_Term** | Term of the loan in months |
| **Credit_History** | 1.0 (Good) or 0.0 (Poor) |
| **Property_Area** | Urban / Semi-Urban / Rural |
| **Loan_Status** | **(Target)** Y (Approved) / N (Rejected) |

---

## ⚙️ Project Workflow

### 1. Data Preprocessing
* **Handled Missing Data:** Used statistical imputation (Mean/Mode) for features like `LoanAmount` and `Credit_History`.
* **Outlier Treatment:** Applied **Log Transformations** to normalize skewed distributions in income and loan amounts.
* **Feature Encoding:** Converted categorical text data into numerical values using **Label Encoding** for model compatibility.

### 2. Exploratory Data Analysis (EDA)
* Identified that `Credit_History` is the most significant factor in loan approval.
* Visualized the impact of **Education** and **Marital Status** on loan success rates.
* Analyzed income distribution using **Box Plots** and **Histograms**.

### 3. Model Building
Implemented and compared the following algorithms:
* **Logistic Regression** (Baseline model)
* **Decision Tree**
* **Random Forest**

---

## 📊 Results & Insights
* **Top Predictor:** Applicants with a `Credit_History` of **1.0** have an exponentially higher chance of approval.
* **Socio-Economic Factors:** Graduates and married applicants tend to have higher loan approval rates in this specific dataset.
* **Model Accuracy:** The final model achieved high predictive accuracy, effectively balancing precision and recall for the "Approved" class.

---

## 🛠️ Technologies Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
* **Environment:** Jupyter Notebook

---

## 📁 Project Structure
```plaintext
├── data/
│   └── loan_data.csv           # Raw dataset
├── loan_prediction.ipynb       # Full Python implementation & EDA
├── loan_prediction.html        # Exported report of the analysis
└── README.md                   # Project documentation
```
---

## 📌 Conclusion

This project demonstrates the power of classification algorithms in the fintech sector. By automating the loan approval process, banks can reduce manual labor and focus on high-risk cases, ultimately improving operational efficiency and customer experience.
