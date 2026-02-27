# Medical-Insurance-Cost-Analysis-Prediction
## 📌 Project Overview
This project presents a comprehensive statistical analysis of medical insurance costs using demographic, lifestyle, and policy-related data.  
The analysis is motivated by rising healthcare and insurance costs, with the objective of identifying key risk factors that significantly influence insurance charges.

The project focuses on data cleaning, exploratory data analysis (EDA), inferential statistics, and confidence interval estimation to support data-driven pricing decisions for an insurance company.

---

## 🎯 Objectives
- Clean and prepare a real-world insurance dataset with missing values and inconsistencies  
- Explore relationships between demographic/lifestyle factors and medical charges  
- Identify statistically significant cost drivers using hypothesis testing  
- Estimate the true average insurance cost using confidence intervals  
- Provide actionable insights for insurance pricing and risk management  

---

## 📂 Dataset Description
The dataset contains **1,338 insurance beneficiaries** and includes the following variables:

| Feature | Description |
|-------|------------|
| age | Age of the primary beneficiary |
| gender | Gender of the beneficiary |
| bmi | Body Mass Index |
| children | Number of dependents covered |
| smoker | Smoking status (yes/no) |
| region | Residential region |
| noclaimsbonus | No-Claims Bonus (5%–20%) |
| charges | Medical insurance charges |

---

## 🧹 Data Cleaning & Preparation
Key data preprocessing steps included:

- Corrected misspelled categorical values in the `region` column  
- Removed rows with missing values (less than 5% of the dataset)  
- Converted `children` from float to integer  
- Standardized column naming conventions  
- Detected and handled outliers using the IQR method  
  - Implausible values in `children` were removed  
  - High medical charges and BMI outliers were retained as realistic  

Final dataset size after cleaning: **1,313 records**

---

## 📊 Exploratory Data Analysis (EDA)
EDA was conducted to understand the distribution of variables and uncover patterns:

### Key Findings:
- Medical charges are **right-skewed**, with a small number of very high-cost claims  
- The average BMI falls into the **obese** category, indicating elevated health risk  
- The Southeast region shows higher variability in medical costs  
- Smokers incur significantly higher charges than non-smokers  

Visualizations included:
- Histograms and KDE plots  
- Boxplots by region, gender, smoking status, and number of children  
- Correlation heatmap and pair plots  

---

## 📈 Inferential Statistics

### Hypothesis Testing

#### 1️⃣ Smoking Status vs Medical Charges
- **Test:** Independent Samples T-test  
- **Result:** Statistically significant difference (p < 0.001)  
- **Conclusion:** Smoking is the strongest cost driver in the dataset  

#### 2️⃣ Gender vs Medical Charges
- **Test:** Independent Samples T-test  
- **Result:** Statistically significant but small effect (p ≈ 0.02)  
- **Conclusion:** Gender differences exist but are likely influenced by confounding factors  

---

## 📐 Confidence Interval Estimation
A 95% confidence interval was calculated to estimate the true population mean of medical charges.

- **Sample Mean:** \$13,260  
- **95% Confidence Interval:** \$12,605 – \$13,916  

**Interpretation:**  
We are 95% confident that the true average medical insurance cost lies within this range, providing a reliable benchmark for financial planning.

---

## 🧠 Key Insights
- Smoking status is the dominant determinant of medical insurance costs  
- BMI and age show moderate positive relationships with charges  
- Regional differences exist but are less influential than lifestyle factors  
- Premium pricing should prioritize behavioral and health indicators over demographics  

---

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- Jupyter Notebook
- GitHub (Project documentation & version control)

---

## 📁 Project Structure
├── insurance_analysis.ipynb   # Main Jupyter Notebook with all analysis, EDA, and visualizations
├── insurance_data.xlsx        # Dataset used for analysis
└── README.md                  # This README file

---


---

## 👤 Author
**Baasankhuu**  
Aspiring Data Analyst | Python • Data Visualization • Statistics • SQl • Power BI
