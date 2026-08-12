# 🏦 Bank Loan & Credit Risk Analysis — EDA

## 📌 Project Overview

This project presents an Exploratory Data Analysis (EDA) of **45,000 bank loan applications** to understand borrower characteristics, loan patterns, credit profiles, and loan outcomes.

The analysis focuses on variables such as applicant income, employment experience, home ownership, loan purpose, loan amount, interest rate, credit score, previous loan defaults, and loan status.

The objective is to identify meaningful patterns within the loan portfolio and generate data-driven insights that can support better understanding of credit risk.

---

## 🎯 Project Objectives

* Understand the structure and characteristics of the loan dataset.
* Inspect and clean the available data.
* Process variables for analysis.
* Create meaningful analytical features.
* Analyze loan outcomes across customer and loan characteristics.
* Identify patterns associated with loan defaults.
* Generate actionable business insights and recommendations.

---

## 📂 Dataset

The analysis uses the **Bank Loan Data** dataset containing:

* **45,000 rows**
* **14 original columns**

### Main Variables

| Category  | Variables                               |
| --------- | --------------------------------------- |
| Customer  | Age, Gender, Education                  |
| Financial | Income, Employment Experience           |
| Housing   | Home Ownership                          |
| Loan      | Loan Amount, Loan Intent, Interest Rate |
| Credit    | Credit Score, Credit History Length     |
| Risk      | Previous Loan Defaults                  |
| Outcome   | Loan Status                             |

**Dataset Source:** Kaggle — Bank Loan Data

---

## 🛠️ Tools & Technologies

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Kaggle Notebook**
* **GitHub**

No machine learning models were used because this project focuses specifically on **Exploratory Data Analysis**.

---

## 🔍 Project Workflow

```text
Data Collection
      ↓
Data Understanding
      ↓
Data Inspection
      ↓
Data Cleaning
      ↓
Data Processing
      ↓
Feature Engineering
      ↓
Exploratory Data Analysis
      ↓
Business Questions
      ↓
Business Insights
      ↓
Recommendations
      ↓
Conclusion
```

---

## 📊 Business Questions

The analysis answers six key business questions:

### Q1. What is the overall distribution of loan outcomes?

The dataset contains **45,000 loan applications**.

* Non-Default: **35,000 (77.78%)**
* Default: **10,000 (22.22%)**

---

### Q2. Which loan purposes are most common among applicants?

Education loans were the most common purpose:

* Education: **9,153 (20.34%)**
* Medical: **8,548 (19.00%)**
* Venture: **7,819 (17.38%)**
* Personal: **7,552 (16.78%)**
* Debt Consolidation: **7,145 (15.88%)**
* Home Improvement: **4,783 (10.63%)**

---

### Q3. How does applicant income vary across loan outcomes?

| Loan Outcome | Average Income | Median Income |
| ------------ | -------------: | ------------: |
| Non-Default  |      86,157.04 |        72,928 |
| Default      |      59,886.10 |        50,629 |

Defaulted applicants had considerably lower income levels than non-defaulted applicants.

---

### Q4. How does credit score relate to loan outcomes?

Average credit scores were very similar:

| Loan Outcome | Average Credit Score |
| ------------ | -------------------: |
| Default      |               631.89 |
| Non-Default  |               632.81 |

The analysis suggests that **credit score alone does not strongly differentiate default and non-default outcomes** in this dataset.

---

### Q5. Which loan purposes have the highest default rates?

| Loan Purpose       | Default Rate |
| ------------------ | -----------: |
| Debt Consolidation |   **30.27%** |
| Medical            |   **27.82%** |
| Home Improvement   |   **26.30%** |
| Personal           |   **20.14%** |
| Education          |   **16.96%** |
| Venture            |   **14.43%** |

Debt Consolidation loans recorded the highest default rate, while Venture loans recorded the lowest.

---

### Q6. How do loan amount and interest rate vary across loan outcomes?

| Loan Characteristic   |   Default | Non-Default |
| --------------------- | --------: | ----------: |
| Average Loan Amount   | 10,855.69 |    9,219.58 |
| Median Loan Amount    |     9,750 |       8,000 |
| Average Interest Rate |    12.86% |      10.48% |
| Median Interest Rate  |    12.98% |      10.85% |

Defaulted applicants generally had **larger loans and higher interest rates**.

---

## 💡 Key Business Insights

1. **22.22% of applicants were classified as defaulted**, highlighting a meaningful level of credit risk within the dataset.

2. **Education loans represented the largest share of applications at 20.34%**, followed by Medical loans at 19.00%.

3. Defaulted applicants had a substantially lower average income (**59,886.10**) compared with non-defaulted applicants (**86,157.04**).

4. Credit scores were almost identical between defaulted and non-defaulted applicants, suggesting that credit score alone may not explain loan outcomes.

5. **Debt Consolidation had the highest default rate at 30.27%**, while Venture loans had the lowest at 14.43%.

6. Defaulted applicants had higher average loan amounts (**10,855.69**) compared with non-defaulted applicants (**9,219.58**).

7. Defaulted applicants also had higher average interest rates (**12.86%**) compared with non-defaulted applicants (**10.48%**).

---

## 🎯 Business Recommendations

### 1. Strengthen Monitoring of High-Risk Loan Purposes

Debt Consolidation, Medical, and Home Improvement loans showed relatively high default rates and could receive additional risk monitoring.

### 2. Consider Income During Credit Assessment

Income showed a noticeable difference between defaulted and non-defaulted applicants and should remain an important consideration when assessing repayment capacity.

### 3. Review Higher Loan Amounts Carefully

Higher loan amounts were associated with defaulted applicants in the analysis. Additional affordability checks could be considered for larger loan requests.

### 4. Evaluate Interest Rates Alongside Repayment Capacity

Higher interest rates were observed among defaulted applicants. Lending decisions should consider whether the proposed repayment obligation is affordable for the borrower.

### 5. Avoid Relying on Credit Score Alone

Credit scores were very similar between the two outcome groups. A broader assessment using income, loan purpose, loan amount, interest rate, and previous loan history may provide better risk evaluation.

---

## ⚠️ Limitations

* The analysis identifies relationships and patterns but does not establish causation.
* The dataset may not represent every banking customer or lending market.
* Some categories contain relatively few observations.
* The analysis is limited to the variables available in the dataset.
* No predictive machine learning model was developed because this project focuses on EDA.

---

## 📝 Conclusion

This project analyzed **45,000 bank loan applications** to identify patterns in borrower characteristics, loan characteristics, and loan outcomes.

The analysis found that defaulted applicants generally had **lower incomes, larger loan amounts, and higher interest rates** than non-defaulted applicants.

Loan purpose also showed a meaningful relationship with default rates, with **Debt Consolidation recording the highest default rate at 30.27%**.

At the same time, credit scores were very similar between defaulted and non-defaulted applicants, demonstrating that a single metric may not be sufficient to understand credit risk.

Overall, the project demonstrates how exploratory data analysis can transform raw financial data into practical business insights that can support better risk monitoring and lending decisions.

---

## 📁 Repository Structure

```text
bank-loan-credit-risk-eda/
│
├── Bank_Loan_Credit_Risk_EDA.ipynb
├── README.md
└── dataset/
    └── README.md
```

---

## 📚 References

* Kaggle — Bank Loan Data
* Pandas Documentation
* NumPy Documentation
* Matplotlib Documentation

---

## 👤 Author

**L Shubham**

Data Analyst | Python | SQL | Power BI | Excel | Tableau

GitHub: `https://github.com/shubham-lingam`
