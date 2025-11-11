# 🧠 Student Stress Analysis

### 📘 **Project Overview**
This project explores factors influencing student stress levels using data collected from 106 student responses.  
Each factor (such as sleep quality, study load, and academic performance) is rated on a scale of **1 to 5**, with **stress level** as the target variable.  

The analysis involves:
- Cleaning and preprocessing the dataset  
- Performing **Exploratory Data Analysis (EDA)** using visualizations  
- Interpreting relationships between different factors and stress levels  

---

### 🎯 **Objective**
To identify which factors most strongly affect student stress levels and uncover actionable insights that can help improve academic well-being.

---

### 🧩 **Dataset Description**

| Column | Description |
|---------|--------------|
| `sleep_quality` 😴 | Self-rated sleep quality (1 = poor, 5 = excellent) |
| `headaches_per_week` 🤕 | Frequency of headaches per week |
| `academic_performance` 👩‍🎓 | Self-rated academic performance |
| `study_load` | Perceived workload intensity |
| `extracurricular_freq` 🎾 | Frequency of extracurricular activities |
| `stress_level` | Overall perceived stress level (target variable) |

- Total entries: **106**  
- Missing values: **0**  
- Duplicates: **Removed**  
- Data type: All numeric (1–5 ordinal scale)

---

### 📊 **Exploratory Data Analysis (EDA)**

#### 1️⃣ Univariate Analysis
Count plots show how each variable is distributed across responses:
- Most students report **moderate sleep quality** and **average academic performance**.
- **Stress levels** are evenly spread, allowing balanced analysis.
- **Study load** tends to skew slightly toward higher values.

#### 2️⃣ Bivariate Analysis
Boxplots reveal how stress level changes with other factors:

| Factor | Relationship | Interpretation |
|--------|---------------|----------------|
| **Sleep Quality** | Negative | Poor sleep correlates with higher stress. |
| **Headaches per Week** | Positive (non-linear) | Headache frequency generally rises with stress, slight dip at level 4. |
| **Academic Performance** | Negative | High stress corresponds to lower academic performance. |
| **Study Load** | Positive | Heavier workload strongly increases stress. |
| **Extracurricular Frequency** | Weak Negative | Students with more extracurriculars report slightly less stress. |

---

### 🌡️ **Correlation Heatmap**
| Feature | Correlation with Stress | Relationship |
|----------|------------------------|---------------|
| **Study Load** | **+0.39** | Most influential factor on stress |
| **Sleep Quality** | **–0.17** | Poor sleep = higher stress |
| **Academic Performance** | +0.06 | Weak correlation |
| **Headaches per Week** | –0.07 | Slightly negative / non-linear |
| **Extracurricular Frequency** | +0.05 | Minimal relationship |

🧠 **Insight:**  
> Study load has the strongest positive correlation with stress, while sleep quality shows a mild negative relationship. Other variables have limited influence individually.

---

### 📈 **Key Insights**
- Heavy **study load** is the top contributor to stress.  
- **Sleep quality** and **headache frequency** also play meaningful roles.  
- **Academic performance** declines as stress increases.  
- Students with **higher extracurricular activity** levels show slightly lower stress.  

---

### 🧮 **Tools & Libraries Used**
- **Python 3.13**  
- **pandas**, **numpy** — Data cleaning & preprocessing  
- **matplotlib**, **seaborn** — Data visualization  
- *(Optional upcoming)*: **scikit-learn** — for predictive modeling  

---

### 🔜 **Next Steps**
- Encode categorical variables (if any)
- Build predictive models (Random Forest, Logistic Regression)
- Evaluate accuracy, confusion matrix, and feature importance

---

### 💬 **Conclusion**
The analysis shows that academic workload and poor sleep habits are major drivers of student stress.  
By managing study load and promoting better sleep routines, institutions can help reduce stress and improve student performance and well-being.

---

### 👨‍💻 **Author**
**Sasivadhan Kandregula**  
Master’s in Computer Science | Seattle University  
GitHub: [Sasivadhan163](https://github.com/Sasivadhan163)
