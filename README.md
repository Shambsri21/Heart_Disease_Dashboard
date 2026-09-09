# Heart_Disease_Dashboard

<img width="770" height="433" alt="image" src="https://github.com/user-attachments/assets/756641d7-1237-410b-b0f2-26476f3624c4" />


# ❤️ Heart Disease Dashboard — End-to-End Project Documentation

## 1. Project Overview

**Project Name:** Heart Disease Risk & Patient Survival Analysis
**Tool:** Microsoft Power BI
**Domain:** Healthcare Analytics
**Dataset:** Heart Disease Clinical Records
**Dashboard Type:** Interactive Healthcare KPI & Patient Outcome Dashboard

This project analyzes clinical records of heart-disease patients to understand **survival outcomes, mortality, age-wise patient distribution, cancer-related survival, serum sodium levels, diabetes distribution, and gender-wise patterns**.

The dashboard converts raw clinical data into an interactive visual report that can help identify important patterns in patient outcomes and risk factors.

---

# 2. Project Objective

The primary objectives of this project are:

* Analyze the overall **alive vs. death outcomes**.
* Calculate the **percentage of surviving patients**.
* Understand the **average age of surviving patients**.
* Analyze **average serum sodium levels** across age groups.
* Examine the relationship between **cancer and surviving patients**.
* Analyze the number of surviving patients across different **age groups**.
* Understand the distribution of **diabetes among surviving patients**.
* Provide **gender-based filtering** for deeper analysis.
* Build an easy-to-understand healthcare dashboard for decision-making.

---

# 3. Dataset Information

The dashboard uses a **Heart Disease Clinical Records** dataset.

### Dataset fields available

| Column                | Description                        |
| --------------------- | ---------------------------------- |
| `age`                 | Age of the patient                 |
| `cancer`              | Cancer-related indicator           |
| `count`               | Record/count field                 |
| `DEATH_EVENT`         | Indicates whether the patient died |
| `diabetes`            | Diabetes indicator                 |
| `ejection_fraction`   | Heart pumping efficiency indicator |
| `Gender`              | Gender category                    |
| `Group`               | Age-group/category field           |
| `high_blood_pressure` | High blood pressure indicator      |
| `Hypertension`        | Hypertension indicator             |
| `kidney_marker`       | Kidney-related clinical indicator  |
| `muscle_damage_scale` | Muscle damage measurement          |
| `platelets`           | Platelet count                     |
| `serum_sodium`        | Serum sodium level                 |
| `sex`                 | Sex category                       |
| `time`                | Follow-up/survival time            |

---

# 4. Data Preparation

The data preparation process in Power BI can be divided into the following stages:

### Step 1 — Import Data

The clinical records dataset was imported into **Power BI Desktop**.

### Step 2 — Data Cleaning

The following checks were performed:

* Checked column data types.
* Verified numerical fields.
* Checked categorical fields.
* Checked missing/null values.
* Reviewed duplicate records.
* Standardized gender/sex categories.
* Verified `DEATH_EVENT` values.
* Verified diabetes and cancer indicators.
* Checked age-group categorization.

### Step 3 — Data Transformation

Age groups were created to make the analysis easier.

The dashboard contains the following age groups:

* Below 40
* 40–50
* 50–60
* 60–70
* 70+

---

# 5. Data Modeling

The dashboard appears to use a relatively simple clinical-record structure, where the main table contains the patient-level clinical attributes.

### Main analytical fields

**Demographics**

* Age
* Gender
* Sex
* Age Group

**Medical Conditions**

* Diabetes
* Cancer
* Hypertension
* High Blood Pressure
* Kidney Marker

**Clinical Measurements**

* Serum Sodium
* Platelets
* Ejection Fraction
* Muscle Damage Scale

**Outcome**

* `DEATH_EVENT`
* `time`

---

# 6. KPI Cards

The dashboard contains **five major KPI cards**.

### KPI 1 — Alive %

**Dashboard Value: 67.89%**

This KPI represents the percentage of patients who were alive in the dataset.

**Purpose:**
Helps understand the overall survival proportion of the patients.

### KPI 2 — Alive Average Age

**Dashboard Value: 60.83**

This represents the **average age of patients who were alive**.

**Purpose:**
Helps understand the typical age of surviving patients.

### KPI 3 — Total Alive

**Dashboard Value: 203**

This represents the total number of patients classified as alive.

**Purpose:**
Provides an absolute count of surviving patients.

### KPI 4 — Total Death

**Dashboard Value: 96**

This represents the total number of patients who experienced the death event.

**Purpose:**
Provides the overall mortality count.

### KPI 5 — Average Serum

**Dashboard Value: 60.83 is not the serum KPI; the dedicated serum visual shows age-group values around 136–138.**

The dashboard also contains an **Average of Serum** analysis showing serum sodium values by age group.

---

# 7. KPI Summary

| KPI                   |       Dashboard Value | Business Meaning                    |
| --------------------- | --------------------: | ----------------------------------- |
| **Alive %**           |            **67.89%** | Percentage of patients who survived |
| **Alive Average Age** |             **60.83** | Average age of surviving patients   |
| **Total Alive**       |               **203** | Number of surviving patients        |
| **Total Death**       |                **96** | Number of death events              |
| **Average Serum**     | ~136–138 by age group | Average serum sodium level          |

> **Important:** The dashboard's visible KPI cards are **Alive %, Alive Avg, Total Alive, and Total Death**. The serum analysis is presented as a chart rather than a separate top KPI card.

---

# 8. Dashboard Visual Analysis

## A. Total Alive Cancer

The **Total Alive Cancer** visual compares surviving patients across the age groups.

Values visible in the dashboard are approximately:

| Age Group | Alive Cancer |
| --------- | -----------: |
| Below 40  |            7 |
| 70+       |           52 |
| 40–50     |           67 |
| 60–70     |           85 |
| 50–60     |           88 |

### Key Observation

The **50–60 age group has the highest value at 88**, followed by the **60–70 group with 85**.

The Below-40 group has the lowest value at **7**.

---

# 9. Average Serum by Age Group

The dashboard analyzes the average serum sodium level across age groups.

| Age Group | Average Serum |
| --------- | ------------: |
| Below 40  |    **137.71** |
| 50–60     |    **137.03** |
| 60–70     |    **136.82** |
| 40–50     |    **136.18** |
| 70+       |    **136.04** |

### Key Observation

The serum sodium values are relatively close across the age groups, ranging approximately from **136.04 to 137.71**.

The **Below-40 group shows the highest average serum value (137.71)**, while the **70+ group shows the lowest (136.04)**.

---

# 10. Total Alive by Age Group

This visual provides the number of surviving patients by age group.

| Age Group | Total Alive |
| --------- | ----------: |
| 60–70     |      **64** |
| 50–60     |      **63** |
| 40–50     |      **48** |
| 70+       |      **21** |
| Below 40  |       **7** |

### Key Observation

The largest number of surviving patients belongs to the:

**60–70 age group → 64 patients**

followed by:

**50–60 → 63 patients**

The **Below-40 group has only 7 surviving patients**.

---

# 11. Total Alive and Diabetes Distribution

The donut chart shows:

* **118 patients — 58.13%**
* **85 patients — 41.87%**

### Interpretation

The dashboard indicates that the two diabetes categories account for:

| Category   | Patients | Percentage |
| ---------- | -------: | ---------: |
| Category 1 |      118 |     58.13% |
| Category 2 |       85 |     41.87% |
| **Total**  |  **203** |   **100%** |

Because the field is named `diabetes`, the exact category interpretation should be confirmed from the source data's coding (for example, whether `1 = Yes` and `0 = No`) before presenting the categories as "Diabetic" and "Non-Diabetic."

---

# 12. Gender Analysis

The dashboard includes gender filters:

* **Female**
* **Male**

These slicers allow users to dynamically analyze:

* Alive %
* Total Alive
* Total Death
* Age-group distribution
* Cancer-related survival
* Diabetes distribution
* Serum sodium

by gender.

### Example

Selecting **Male** will filter the entire dashboard to male patients.

Selecting **Female** will filter the entire dashboard to female patients.

This makes the dashboard interactive rather than a static report.

---

# 13. Recommended DAX Measures

Based on the fields visible in the Power BI model, the following measures can be used.

### Total Patients

```DAX
Total Patients =
COUNTROWS('heart_Disease_clinical_records_')
```

### Total Alive

```DAX
Total Alive =
CALCULATE(
    COUNTROWS('heart_Disease_clinical_records_'),
    'heart_Disease_clinical_records_'[DEATH_EVENT] = 0
)
```

### Total Death

```DAX
Total Death =
CALCULATE(
    COUNTROWS('heart_Disease_clinical_records_'),
    'heart_Disease_clinical_records_'[DEATH_EVENT] = 1
)
```

### Alive %

```DAX
Alive % =
DIVIDE(
    [Total Alive],
    [Total Patients],
    0
)
```

Format this measure as **Percentage**.

### Alive Average Age

```DAX
Alive Average Age =
CALCULATE(
    AVERAGE('heart_Disease_clinical_records_'[age]),
    'heart_Disease_clinical_records_'[DEATH_EVENT] = 0
)
```

### Average Serum

```DAX
Average Serum =
AVERAGE(
    'heart_Disease_clinical_records_'[serum_sodium]
)
```

### Total Alive Cancer

If `cancer = 1` represents cancer:

```DAX
Total Alive Cancer =
CALCULATE(
    COUNTROWS('heart_Disease_clinical_records_'),
    'heart_Disease_clinical_records_'[DEATH_EVENT] = 0,
    'heart_Disease_clinical_records_'[cancer] = 1
)
```

### Total Alive Diabetes

```DAX
Total Alive Diabetes =
CALCULATE(
    COUNTROWS('heart_Disease_clinical_records_'),
    'heart_Disease_clinical_records_'[DEATH_EVENT] = 0,
    'heart_Disease_clinical_records_'[diabetes] = 1
)
```

> The exact DAX should be adjusted if your dataset uses different coding for `cancer`, `diabetes`, or `DEATH_EVENT`.

---

# 14. Dashboard Design

The dashboard follows a **medical/healthcare theme** with:

* Dark background
* Red cardiovascular theme
* Heart illustration
* KPI cards
* Bar charts
* Donut chart
* Gender slicers
* Consistent rounded-card design
* High-contrast KPI values

### Dashboard Structure

**Top Section**

* Alive %
* Alive Average Age
* Total Alive
* Total Death

**Left Section**

* Heart visual
* Gender filters

**Middle/Right Section**

* Total Alive Cancer
* Average Serum
* Total Alive by Age Group
* Diabetes distribution

This layout provides a clear **executive summary → demographic analysis → clinical analysis** flow.

---

# 15. Key Business/Healthcare Insights

Based on the dashboard:

### 1. Majority of patients are alive

The dashboard shows an **Alive % of 67.89%**, indicating that approximately two-thirds of the analyzed patients were alive.

### 2. Mortality remains significant

There are **96 recorded deaths**, compared with **203 surviving patients**.

### 3. Surviving population is concentrated around 50–70

The largest surviving groups are:

* 60–70 → **64**
* 50–60 → **63**
* 40–50 → **48**

Together, these groups represent the majority of surviving patients.

### 4. Younger patients have fewer records

The Below-40 group has only **7 surviving patients**, which is considerably lower than the other age groups.

### 5. Serum sodium is relatively stable

Average serum sodium ranges approximately from:

**136.04 to 137.71**

across the displayed age groups.

### 6. Diabetes distribution is uneven

The dashboard shows a split of:

**118 patients (58.13%) vs. 85 patients (41.87%)**

within the alive population.

---

# 16. Important Dashboard Questions Answered

The dashboard can answer questions such as:

1. What percentage of patients survived?
2. How many patients are alive?
3. How many patients died?
4. What is the average age of surviving patients?
5. Which age group has the highest number of surviving patients?
6. Which age group has the lowest number of surviving patients?
7. How does cancer-related survival vary by age group?
8. What is the average serum sodium level by age group?
9. How is diabetes distributed among surviving patients?
10. How do the results change for males versus females?

---

# 17. End-to-End Project Workflow

```text
Raw Clinical Dataset
        ↓
Data Import
        ↓
Power Query
        ↓
Data Cleaning
        ↓
Data Transformation
        ↓
Age Group Creation
        ↓
Data Modeling
        ↓
DAX Measures
        ↓
KPI Development
        ↓
Visual Analysis
        ↓
Interactive Filters
        ↓
Dashboard Design
        ↓
Healthcare Insights
        ↓
Business Recommendations
```

---

# 18. Tools & Technologies

### Microsoft Power BI

Used for:

* Data transformation
* Data modeling
* DAX calculations
* Interactive visualizations
* Dashboard development

### Power Query

Used for:

* Data cleaning
* Data type correction
* Null-value handling
* Transformation
* Creating calculated categories

### DAX

Used for:

* KPI calculations
* Survival percentage
* Alive/death counts
* Average age
* Average serum
* Conditional analysis

---

# 19. Skills Demonstrated

This project demonstrates the following **Data Analyst skills**:

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Transformation
* Data Modeling
* KPI Development
* Healthcare Data Analysis
* Interactive Dashboard Development
* Data Visualization
* Business/Analytical Insight Generation

---

# 20. Project Limitations

This dashboard is intended for **analytical and educational purposes**, not clinical diagnosis.

Some important limitations include:

* The dataset represents recorded observations and may not represent the general population.
* Correlation between a clinical variable and death should not automatically be interpreted as causation.
* Binary fields such as diabetes and cancer require confirmation of their underlying coding.
* The dashboard alone cannot determine medical treatment recommendations.
* Additional clinical variables would be required for comprehensive risk prediction.

---

# 21. Future Enhancements

The project could be further improved by adding:

### Advanced KPIs

* Mortality Rate
* Survival Rate by Gender
* Average Follow-up Time
* Average Ejection Fraction
* High Blood Pressure %
* Diabetes %
* Hypertension %

### Advanced Visuals

* Mortality by age group
* Survival trend by follow-up time
* Ejection fraction vs. survival
* Diabetes vs. mortality
* Hypertension vs. mortality
* Cancer vs. mortality
* Kidney marker vs. survival

### Advanced Power BI Features

* Drill-through patient analysis
* Tooltip pages
* Bookmarks
* Dynamic titles
* Field parameters
* What-if analysis
* Conditional formatting
* Dynamic KPI cards

---

# 22. Portfolio/Resume Project Description

### **Heart Disease Risk & Patient Survival Analysis | Power BI**

> Developed an interactive Power BI healthcare dashboard to analyze patient survival and mortality outcomes using clinical records. Created DAX-based KPIs including **67.89% survival rate, 203 surviving patients, 96 death events, and 60.83 average age of surviving patients**. Analyzed age-wise survival, cancer-related outcomes, serum sodium levels, diabetes distribution, and gender-based patterns using interactive visualizations and slicers.

### Resume Bullet Points

* Developed an interactive **Power BI Heart Disease Dashboard** analyzing **299 clinical patient records** with survival, mortality, demographic, and clinical indicators.
* Created DAX measures for **Alive %, Total Alive, Total Death, Average Age, and Average Serum Sodium**.
* Built age-group, cancer, diabetes, serum sodium, and gender analyses to identify meaningful patient-outcome patterns.
* Applied **Power Query, DAX, data modeling, and interactive visualization techniques** to transform clinical data into actionable insights.

---

# 23. Final Project Summary

**Heart Disease Risk & Patient Survival Analysis** is an end-to-end Power BI project that transforms clinical patient data into an interactive healthcare analytics dashboard.

The dashboard provides a high-level view of **survival, mortality, age distribution, cancer, diabetes, serum sodium, and gender-based patterns**.

The most important dashboard KPIs are:

> 🟢 **Alive % — 67.89%**
> 👤 **Total Alive — 203**
> ⚰️ **Total Death — 96**
> 📊 **Alive Average Age — 60.83**
> 🧪 **Average Serum Sodium — approximately 136–138 across age groups**


