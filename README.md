# Codealpha_task2
#  TASK 2: Exploratory Data Analysis (EDA) – Titanic Dataset

This repository contains the EDA performed on the Titanic dataset as part of my internship task.

## Task Objectives

✔️ Ask meaningful questions about the dataset  
✔️ Explore the data structure, including variables and data types  
✔️ Identify trends, patterns, and anomalies  
✔️ Test hypotheses and validate assumptions using statistics and visualization  
✔️ Detect potential data issues for further analysis  

---

## Questions Explored

1. What percentage of passengers survived?
2. Did survival chances differ by gender?
3. Did passenger class affect survival rate?
4. Were children more likely to survive?
5. How are Fare and Age distributed? Are there any outliers?

---

##  Data Structure & Cleaning

- Data Source: [`train.csv`](data/train.csv)
- Missing values:
  - Age: Filled with median
  - Embarked: Filled with mode
  - Cabin: Dropped due to too many missing entries
- Categorical Variables: Sex, Embarked
- Numerical Variables: Age, Fare, SibSp, Parch

---

## Visualizations

- Count plots for Survival, Gender, Pclass
- Histogram of Age
- Boxplots for Fare and Age
- Correlation heatmap


##  Hypotheses Tested

| Hypothesis | Result |
|------------|--------|
| Females were more likely to survive | ✅ True |
| 1st class passengers had better survival | ✅ True |
| Children (Age < 12) had higher survival | ✅ True |
| Fare is right-skewed | ✅ True |
| Age is symmetric or slightly right-skewed | ✅ Mostly True |

---

##  Data Issues Detected

- Outliers in Fare (extremely high)
- Some missing data in Age, Embarked
- Cabin not usable due to 77% missing

---

##  Repository Structure

Codealpha_task2/
├── data/
│   └── train.csv
├── titanic_eda.ipynb
├── README.md
├── images/
│   └── (your plot images)
└── requirements.txt

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

## Conclusion

This EDA helped uncover key survival patterns and prepare the dataset for machine learning models. The cleaned dataset and findings are ready for further predictive analysis.


