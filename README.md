# Analyzing Factors Influencing COVID-19 Severity and Vaccination Uptake in the United States

## Overview
This project identifies patterns in socio-economic and demographic factors that shape COVID-19 severity and vaccination uptake. By analyzing data such as age, sex, race, and vaccination metrics, we aim to provide actionable insights for public health improvements. The study focuses on reducing disparities, enhancing population immunity, and preparing for future health crises.

---

## Business Problem
To identify patterns in socio-economic and demographic factors that influence COVID-19 severity and vaccination uptake, providing actionable insights for public health strategies. Key factors analyzed include:

- **Race & Ethnicity**
- **Age**
- **Gender**

---

## CRISP-DM Framework
The project follows the CRISP-DM framework:

1. **Business Understanding**
2. **Data Understanding**
3. **Data Preparation and Cleaning**
4. **Modeling**
5. **Evaluation**
6. **Deployment**

---

## Data Sources
The data used in this project comes from the [CDC COVID Data Tracker](https://data.cdc.gov/Vaccinations/COVID-19-Vaccination-Demographics-in-the-United-St/km4m-vcsb/about_data). It includes vaccination and demographic information from various partners such as:

- Jurisdictional clinics
- Retail pharmacies
- Long-term care facilities
- FEMA and HRSA partner sites
- Federal entity facilities

### Dataset Information
- **Rows:** 29,886
- **Columns:** 25

### Key Variables
- **Date:** Reporting date for vaccination and case data
- **Demographic Category:** Categorized by age, sex, or race/ethnicity of vaccine recipients
- **Administered Dose Metrics:** Total count and percentage of individuals receiving at least one vaccine dose
- **Series Completion Metrics:** Total count and percentage of individuals completing the primary vaccination series
- **Booster Metrics:** Total count and percentage of individuals receiving booster doses
- **Total Intake:** A calculated column summing vaccination metrics across all stages

---

## Data Cleaning
- Removed duplicates
- Handled missing values
- Ensured data accuracy and reliability

---

## Data Visualizations

### Key Insights:
1. **Vaccine Intake by Age Group:**
   - Highest intake among "25-49 years"
   - Children under 12 had significantly lower intake

2. **Vaccine Intake by Date and Age:**
   - Steady increase over time, with leading groups being "25-39 years" and "65+ years"

3. **Vaccine Intake by Date and Sex:**
   - Females slightly outpaced males in vaccine uptake

4. **Vaccine Intake Distribution by Sex:**
   - Near-even split between males and females

5. **Total Intake by Age:**
   - "25-49 years" group showed high variability, while older adults ("50-64" and "65+") had consistently high uptake

6. **Vaccine Intake Over Time by Race:**
   - Non-Hispanic Whites lead vaccine uptake, with steady increases across all racial groups

7. **Boxplot Analysis:**
   - Highlights median vaccine intake by age, sex, and race, showing disparities and dominant contributors

---

## Model Building
- **Model:** Random Forest Regression
- **Performance:**
  - R-Squared: 0.9997
  - Mean Absolute Error (MAE): 0.0123
  - Mean Squared Error (MSE): 0.0082

### Top Features Impacting Vaccination:
- **Year:** Most significant predictor, reflecting the temporal progression of vaccine rollouts
- **Age Groups:** Vulnerable age groups (e.g., <5 years, 2-4 years) prioritized for vaccination
- **Race/Ethnicity:** Emphasizes disparities and highlights areas for improved equity
- **Temporal Variation:** Month reflects the impact of public health campaigns

---

## Conclusion
Understanding demographic trends and regional variations is critical for improving vaccine distribution and targeting. Key recommendations include:

- Tailored outreach efforts
- Improved demographic data collection
- Alignment with public health campaigns

A data-driven approach is essential for maximizing vaccine uptake, ensuring equitable distribution, and achieving widespread immunity.

---

## Acknowledgments
This project was completed under the guidance of **Prof. Devin Fensterheim** for the course **DATA 602 - Intro to Data Analysis and Machine Learning**.
