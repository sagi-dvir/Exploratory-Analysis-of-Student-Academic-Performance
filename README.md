# Exploratory Analysis of Student Academic Performance

## 📊 Project Overview

This project explores the academic performance of students using Exploratory Data Analysis (EDA) and a classification model. Leveraging a dataset with over 30,000 student records — including demographic, socio-economic, and activity-related variables — the analysis aims to uncover patterns and potential predictors of academic success in Math, Reading, and Writing.

---

## 📁 Dataset

**Name:** Students Exam Scores: Extended Dataset  
**Source:** [Available on Kaggle](https://www.kaggle.com)  
**Instances:** 30,640  
**Attributes:**
- **Demographics:** Gender, Ethnic Group, Parental Education
- **Socio-economic:** Lunch Type, Weekly Study Hours
- **Activity-based:** Test Preparation, Sports Participation
- **Scores:** Math, Reading, Writing

---

## 🛠 Project Structure

1. **Data Preprocessing**
   - Handled missing values using random imputation with ratio preservation.
   - Applied one-hot encoding to categorical variables.
   - Standardized features using z-scores.

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions and correlations.
   - Highlighted key attributes affecting performance (e.g., parental education, test prep).

3. **Hypothesis Testing**
   - Investigated if sports participation improves academic scores.
   - Used bootstrapping with 5000 simulations.
   - Result: No statistically significant impact found (p-value = 1.0).

4. **Classification Model**
   - **Model Used:** K-Nearest Neighbors (KNN)
   - **Features:** Gender, Ethnic Group, Parental Education, Lunch Type, Weekly Study Hours, Test Prep, Sports
   - **Target Variable:** High average score (OverallMean: 1 if 80–100, 0 otherwise)
   - **Evaluation:** Accuracy ~77%, Recall = 16%

---

## 📈 Key Findings

- **Parental Education & Test Prep** show strong correlation with higher academic scores.
- **Sports Participation** has no statistically significant effect on scores.
- The **KNN classifier** provides fair accuracy but struggles with identifying high performers (low recall).

---

## ⚠ Limitations

- **Missing Data:** Despite imputation, potential for bias.
- **Sampling Bias:** Dataset may not represent broader student populations.
- **External Factors:** No data on mental health, home environment, or long-term outcomes.
- **Modeling Simplification:** Binary classification may obscure subtler score variations.

---

## 🔭 Future Directions

- Include more diverse and contextual data (e.g., socio-economic indicators, learning disabilities).
- Explore longitudinal datasets to study trends over time.
- Apply advanced models (e.g., Random Forests, Gradient Boosting).
- Consider qualitative research for causal insights.

---

## 👨‍💻 Author

**Sagi Dvir**  
Exploratory Data Analyst | Education Researcher

---

## 📎 Appendix

Figures referenced in the full report include:
- Score distribution by ethnic group, lunch type, parental education, and test prep.
- KNN performance metrics and simulation results from hypothesis testing.

