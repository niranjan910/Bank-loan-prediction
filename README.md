# Bank Loan Prediction Analysis

- Author: Niranjan  
- Date: 16 May 2025

---

# Project Background

This project analyzes bank loan applications to identify the key factors influencing loan approval decisions. By evaluating customer demographics, financial history, and property-related features, the goal is to develop data-driven insights that can improve risk assessment, customer targeting, and operational decision-making for financial institutions.

Insights and recommendations are provided on the following key areas:

* **Credit History Risk Impact**
* **Income vs Loan Demand**
* **Demographic Influence**
* **Property Area Trends**
* **Repayment Feasibility**

The Python notebooks used to inspect, clean, and analyze the data can be found here `Bank_Loan_Analysis.ipynb`.  
An executive presentation on Power BI can be found here `Bank Loan Dashboard.pdf`.

---

# Data Structure & Initial Checks

The primary data fields are as follows:

* **Gender**: Male/Female applicant
* **Married**: Marital status
* **Dependents**: Number of dependents
* **Education**: Graduate/Not Graduate
* **Self_Employed**: Employment type
* **Loan_Amount_Term**: Loan repayment term
* **Credit_History**: Track record of past credit behavior
* **Property_Area**: Urban/Semiurban/Rural
* **Loan_Status**: Loan approved (Y/N)
* **LoanAmount**: Requested loan amount
* **overall_income**: Combined income of applicant and co-applicant

---

# Executive Summary

### Overview of Findings

The analysis reveals that applicants with a good credit history and stable income are significantly more likely to receive loan approval. Urban and semiurban applicants tend to have higher approval rates compared to rural areas. Higher loan amounts slightly increase rejection probability, especially when credit history is poor. Income levels and property location together influence approval rates, highlighting the importance of combining financial and demographic profiling.

---

# Insights Deep Dive

### Credit History Risk Impact:

* Applicants with **Credit_History = 1.0** have **high approval rates** (~80%+), regardless of demographics.
* When **Credit_History = 0.0**, approval drops drastically.
* Semiurban areas with good credit profiles show the highest approval rates.

### Income vs Loan Demand:

* When **LoanAmount** is high, applicants with **Very High or High Income** still get approved.
* But **low-income applicants requesting large loans** are mostly rejected.
* Suggests income-to-loan ratio plays a key role in approval decisions.

### Demographic Influence:

* **Married male graduates** have higher approval rates.
* **Unmarried females**, especially those self-employed, have lower chances.
* **Education + Employment Status** combinations reveal lending tendencies based on social profiles.

### Property Area Trends:

* **Semiurban applicants** consistently have the highest loan approval.
* Urban and rural regions show mixed results, with **rural + no credit history** facing heavy rejection.
* Bank’s comfort level seems higher in semiurban zones.

### Repayment Feasibility:

* Longer **Loan_Amount_Term** combined with **larger loan amounts** increases rejections.
* Applicants requesting shorter terms tend to be approved, possibly indicating better repayment capacity.

---

# Recommendations

Based on the analysis above, the following actions are recommended:

* Prioritize applicants with **strong credit history** and **moderate-to-high income** levels.
* Create **custom approval scoring models** that combine credit score, income, and property area.
* Offer **financial literacy** or **credit counseling** programs for rural applicants with poor credit records.
* Use **loan amount-to-income ratios** as part of eligibility screening.
* Consider loan term optimization to reduce rejection rates due to affordability concerns.

---

# Assumptions and Caveats

* Missing values were imputed using mean/mode strategies depending on the column type.
* LoanAmount was grouped using logical bins to better analyze affordability.
* Credit_History values were assumed accurate as they are key predictors.
* The analysis assumes consistent policy across branches; geographic bias may exist.

---

## 📬 Contact

For queries or collaborations:
- **Email:** niranjan991100@gmail.com  
- **LinkedIn:** [Niranjan's Profile](https://www.linkedin.com/in/niranjan-a83517229/)
- **Portfolio**: [Portfolio](https://niranjan910.github.io/NiranjanDataAnalystPortfolio.github.io/)
