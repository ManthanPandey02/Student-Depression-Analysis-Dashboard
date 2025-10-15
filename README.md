# 🧠 Student Depression Analysis Dashboard (Power BI)

## 📘 Overview
The **Student Depression Analysis Dashboard** is an interactive **Power BI** project designed to explore, visualize, and understand the factors influencing **mental health among students in India**.  
By integrating academic, demographic, and lifestyle variables, this dashboard provides a **data-driven, evidence-based analysis** of depression, identifying high-risk groups and key behavioral drivers.

---

## 🎯 Objectives
- Quantify the **prevalence of depression** among students.  
- Identify **academic, financial, and lifestyle factors** contributing to mental distress.  
- Highlight **high-risk demographic and geographic groups**.  
- Enable **data-backed decision-making** for institutions, researchers, and policymakers.  
- Demonstrate how **Power BI** and analytics can drive awareness and intervention strategies.

---

## 🧩 Dataset Description
**Source:** Student Depression Dataset (CSV format)  
**Total Records:** 27,901 students  
**Geographic Scope:** Major and Tier-2 cities across India  

| Category | Columns Included |
|-----------|------------------|
| **Demographic** | Gender, Age, City, Degree, Profession |
| **Academic** | CGPA, Academic Pressure, Study Satisfaction, Job Satisfaction, Work/Study Hours |
| **Lifestyle** | Sleep Duration, Dietary Habits |
| **Psychological** | Financial Stress, Suicidal Thoughts, Family History of Mental Illness |
| **Target Variable** | Depression (0 = No, 1 = Yes) |

---

## ⚙️ Data Processing Steps
Data was prepared and transformed using **Power Query Editor** in Power BI.

### 🧹 Cleaning & Standardization
- Removed null or inconsistent entries.  
- Standardized categorical values (e.g., “Others” → “Other”).  
- Converted text-based numeric fields (e.g., *Age*, *CGPA*) into numbers.  

### 🧮 Feature Engineering
- **SleepHours (Numeric)**: Converted from text categories into hour equivalents.  
- **Age Group**: Created custom bands (`18–19`, `20–22`, `23–25`, etc.).  
- **CGPA Band**: Grouped into intervals (`<6`, `6–6.9`, `7–7.9`, `8–8.9`, `9–10`).  
- **Financial Stress Level**: Categorized as *Low*, *Moderate*, *High*.  
- **IsDepressed Column**: Binary conversion (`TRUE/FALSE`) for analysis.  

---

## 📊 Dashboard Structure

### 🟦 **1. Overview Page**
- Displays total student count (**28K**), depression rate (**58.55%**), average CGPA (**7.66**), and average sleep hours (**6.34**).  
- Highlights depression by **gender**, **age group**, and **CGPA band**.  
- Includes a Top-N city view dynamically adjustable with a slicer.

### 🟩 **2. Academics & Workload**
- Correlates **CGPA** with **Work/Study Hours**.  
- Examines **Depression Rate by Financial Stress** and **Job Satisfaction**.  
- Identifies **academic pressure** as a major depression driver.

### 🟨 **3. Lifestyle & Risk**
- Analyzes **sleep duration** and **dietary habits** versus depression rates.  
- Shows that students sleeping <5 hours or eating unhealthy diets are significantly more prone to depression.  
- Integrates **AI Key Influencers visual** revealing that:
  - ↑ Academic Pressure → 3.27× higher depression likelihood  
  - ↑ Financial Stress → 2.32× higher  
  - Unhealthy Diet → 1.38× higher  
  - Long Study Hours → 1.32× higher  
  - Age ≤ 20 → 1.31× higher  

### 🟥 **4. Geography Page**
- Interactive **map visual** of cities across India.  
- Bubble size = *Depressed Count*, color = *Depression Rate*.  
- **Top City Insights Table** listing City, Total Students, Depression Rate, and Risk Ratio.  
- Reveals that Tier-2 cities like **Agra, Lucknow, and Jaipur** show comparable or higher depression ratios than metros.

### 🟪 **5. Details Page**
- Tabular view for research & data validation.  
- Includes gender, city, degree, academic variables, and mental health indicators for individual records.

---

## 📈 Key Insights

| Category | Key Finding |
|-----------|--------------|
| **Overall Depression Rate** | 58.55% of students affected |
| **Suicidal Thoughts** | 63% of students reported |
| **Gender** | Nearly identical rates (M: 58.63%, F: 58.45%) |
| **Age** | 18–19 years most vulnerable (73.59%) |
| **Academic Pressure** | Highest correlation with depression |
| **Financial Stress** | Students under high stress: 75.6% depression rate |
| **Sleep & Diet** | <5 hours sleep → 64.5% depression; Unhealthy diet → 70.7% |
| **Geography** | Tier-2 cities exhibit similar or higher risk ratios than metros |

---

## 💡 Insights Summary
- **Depression is behavioral and environmental**, not demographic.  
- **Academic and financial stress** are the strongest predictors.  
- **Sleep duration and diet quality** are key modifiable factors.  
- **Younger age groups** are most vulnerable.  
- **Tier-2 cities** are emerging as new mental-health hotspots.

---

## 📍 Conclusion
The **Student Depression Analysis Dashboard** transforms mental-health data into actionable intelligence.  
Findings indicate that **six in ten students** face depressive symptoms, with stress, lifestyle, and academic pressure as primary contributors.  
This highlights a national-level wellbeing crisis that transcends gender and geography.  
The dashboard demonstrates how **data analytics can humanize insights**, enabling universities, NGOs, and policymakers to design **preventive interventions** rather than reactive measures.  
Ultimately, this Power BI project advocates for a holistic approach where education systems promote **both academic excellence and emotional resilience** — using data as a tool to create healthier, more balanced learning environments.

---

## 🧠 Technologies Used
- **Microsoft Power BI Desktop**
- **Power Query (M Language)**
- **DAX (Data Analysis Expressions)**
- **Excel / CSV Data Source**
- **Bing Maps API (Geo visualization)**

---

## 📁 Folder Structure
