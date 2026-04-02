# Titanic EDA
### Day 1 — Data Analysis Fundamentals | Pandas, Seaborn & Matplotlib

---

## Project Overview
This project performs a full Exploratory Data Analysis (EDA)
on the famous Titanic dataset (891 passengers, 12 features).
The goal is to uncover patterns in survival rates based on
passenger characteristics such as age, sex, class, and fare.

---

## Dataset
- **Source:** Titanic Dataset (Kaggle / Seaborn built-in)
- **Samples:** 891 passengers
- **Features:** 12 (age, sex, pclass, fare, embarked, etc.)
- **Target:** Survived (0 = No, 1 = Yes)
- **Survival rate:** ~38% survived

---

## Analysis Performed

### 1. Data Loading & Inspection
- Loaded dataset using Pandas
- Checked shape, data types, and first rows
- Identified missing values across columns

### 2. Missing Value Analysis
| Column | Missing Values |
|---|---|
| Age | 177 (19.9%) |
| Cabin | 687 (77.1%) |
| Embarked | 2 (0.2%) |

### 3. Survival Analysis
- Overall survival rate: 38.4%
- Survival by sex: females survived at 74%, males at 19%
- Survival by class: 1st class 63%, 2nd 47%, 3rd 24%
- Survival by age: children under 10 had highest survival rate

### 4. Key Visualisations
- Survival count plot
- Survival rate by sex
- Survival rate by passenger class
- Age distribution by survival
- Fare distribution
- Correlation heatmap

---

## Key Findings
1. **Sex** was the strongest predictor — women survived
   at nearly 4x the rate of men ("women and children first")
2. **Passenger class** strongly influenced survival —
   1st class passengers had far better access to lifeboats
3. **Age** mattered for children — passengers under 10
   had higher survival regardless of class
4. **Fare** correlates with class and survival — higher
   fares meant higher decks and closer lifeboat access

---

## How to Run

### Install dependencies
```bash
pip install pandas seaborn matplotlib jup
