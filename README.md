# Employee Attrition Analysis & Prediction

##  Project Overview
This project explores employee attrition using HR data and builds a machine learning model to predict whether an employee is likely to leave the company.

The goal is to:
- Understand key factors associated with employee attrition
- Perform exploratory data analysis (EDA)
- Build and evaluate a predictive model
- Communicate insights clearly for business decision-making

---

##  Project Structure

```
employee-attrition-analysis/
│
├── data/
│ └── raw/
│ └── Employee.csv
│
├── notebooks/
│ ├── 01_eda_attrition.ipynb
│ └── 02_attrition_model.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
```


---

##  Dataset
- Source: Public HR dataset
- Rows: ~4,600 employees
- Target variable: `LeaveOrNot`
    - `1` → Employee left
    - `0` → Employee stayed

### Key Features
- Age
- Gender
- Education level
- City
- Payment tier
- Experience in current domain
- Ever benched

---

##  Exploratory Data Analysis (Notebook 01)
The EDA focuses on:
- Class balance of attrition
- Attrition rates by payment tier
- Attrition by age group and gender
- Impact of experience and benching on attrition

Key insights are visualized using bar charts and cross-tabulations.

---

##  Modeling (Notebook 02)
- Target: `LeaveOrNot`
- Train / test split
- Categorical encoding
- Model used: **Random Forest Classifier**
- Evaluation metrics:
    - Accuracy
    - Precision / Recall
    - Confusion matrix

The model is evaluated with an emphasis on interpretability and business relevance rather than raw accuracy alone.

---

##  Key Takeaways
- Attrition rates vary significantly across payment tiers
- Lower payment tiers show higher churn risk
- Age and experience influence attrition but are not the sole drivers
- Machine learning models can help prioritize retention strategies

---

## 🛠 How to Run the Project

```bash
pip install -r requirements.txt
jupyter notebook
