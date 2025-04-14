# 📊 IBM Employee Attrition Prediction – Strategic Analytics Project

This project analyzes IBM HR data to identify key drivers of employee attrition and provides strategic insights to help reduce turnover. Using a machine learning pipeline and interpretability techniques, we uncover patterns that reveal *who is likely to leave* and *why it matters*.

> 🔍 **Objective:** Predict employee attrition and deliver actionable strategies for talent retention using real IBM HR data.

---

## 📁 Dataset Overview
- **Source:** IBM HR Analytics Employee Attrition & Performance dataset (https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Rows:** 1470 employees  
- **Target:** `Attrition` (Yes/No → Converted to binary `Churn`)  
- **Features:** Demographic, compensation, tenure, travel, engagement, job roles, etc.

---

## 🔧 Project Phases

### 1. 📈 Exploratory Data Analysis
- Employees who churn tend to be **younger**, have **lower monthly income** and **work overtime** more frequently.
- **Sales Executives, Research Scientists, and Lab Technicians** show the highest attrition rates.
- Clients with **shorter tenure** and **lower engagement scores** are significantly more likely to churn.

### 2. 🤖 Modeling
- **Model Used:** `RandomForestClassifier`  
- **Accuracy:** `87%`  
- **Precision (Churn class):** `71%`  
- **Top Features:** MonthlyIncome, Age, TotalWorkingYears, OverTime, DistanceFromHome

### 3. 🧠 Feature Importance + Strategic Insights

| Feature              | Importance Score | Strategic Insight                                     |
|----------------------|------------------|-------------------------------------------------------|
| MonthlyIncome        | 0.087            | Higher salaries may help retain employees             |
| Age                  | 0.065            | Younger employees are more likely to churn            |
| TotalWorkingYears    | 0.059            | More total experience reduces churn risk              |
| OverTime             | 0.058            | Overtime is strongly associated with churn            |
| DailyRate            | 0.052            | Pay differences reflect inconsistent compensation     |
| MonthlyRate          | 0.051            | Volatility in pay may affect satisfaction             |
| YearsAtCompany       | 0.047            | Longer tenure usually means higher loyalty            |
| DistanceFromHome     | 0.044            | Greater distance from home increases churn            |
| YearsWithCurrManager | 0.033            | Strong manager relationships reduce churn             |
| MaritalStatus        | 0.029            | Married employees show more retention                 |
--------------------------------------------------------------------------------------------------

## 💡 Key Insights

1. **Compensation is crucial** – MonthlyIncome is the strongest predictor of attrition.
2. **Overtime is a red flag** – Consistently links to high churn risk.
3. **Younger employees churn more** – Early career attrition is significant.
4. **Remote/flex options can help** – Distance from home is a strong factor.
5. **Longer tenure = loyalty** – Employees with time invested are more likely to stay.

---

## 🎯 Strategic Recommendations

| Strategy                     | Description                                                  |
|------------------------------|--------------------------------------------------------------|
| 💰 Compensation Alignment    | Adjust salary bands for high-risk roles and age groups       |
| 🕒 Overtime Reduction        | Monitor and address high overtime workloads                  |
| 🤝 Manager Stability         | Invest in long term manager employee relationships           |
| 🧭 Early-Career Engagement   | Implement mentorship for employees with <2 years at IBM      |
| 🏡 Commute-Aware Flexibility | Remote/hybrid options for long-distance employees            |
----------------------------------------------------------------------------------------------

## 🔍 Tools Used
- Python, Pandas, Matplotlib, Seaborn  
- Scikit-Learn (RandomForestClassifier)  
- Jupyter Notebook  

---

## 💬 Final Thought

> This isn’t just a prediction model, it’s a decision-making toolkit.  
Built with IBM in mind. Focused on retention. Grounded in data.

---
