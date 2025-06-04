
# 📊 HR Attrition Analytics - Power BI Project

## 📝 Overview

This Business Intelligence (BI) project focuses on analyzing **HR attrition** data using **Power BI**, aiming to uncover critical workforce trends and support strategic retention efforts. Over a **4-week timeline**, the BI team collaboratively transformed raw HR data into insightful dashboards and actionable recommendations.

---

## 🚀 Project Objectives

- Identify key drivers of employee attrition.
- Provide a data-driven foundation for HR decision-making.
- Visualize demographic, satisfaction, and performance patterns.
- Recommend strategic initiatives for retention and equity.

---

## 🧑‍💻 Team & Tools

**Team Members:**  
- Ahmed Mohsen (Me)
- Abdulrahman Hasib  
- Ahmed Ibrahim  
- Ibrahim Ahmed  
- Ali Gamal  
- Huda Moussa

**Tools & Technologies Used:**  
- **Power BI**
- **Power Query (M Language)**
- **DAX (Data Analysis Expressions)**
- **Microsoft Excel**
  
---

## 📅 Project Timeline

| Week | Phase                         | Key Activities                                                                 |
|------|-------------------------------|---------------------------------------------------------------------------------|
| 1    | Research & Planning           | Define scope, understand dataset, set communication plans                      |
| 2    | Data Cleaning                 | Remove duplicates, transform columns, create conditionals                      |
| 3    | Modeling & DAX Development   | Build star schema, apply calculated fields and relationships                   |
| 4    | Dashboarding & Finalization | Create dashboards, validate insights, compile recommendations & presentation   |

---

## 📂 Dataset Description

The dataset included employee records with columns such as:
- **Age, Education, Gender, Job Role, Department**
- **Attrition (Yes/No)**
- **ReviewDate, Job Satisfaction, Performance Rating**
- **Business Travel, Overtime, Hire Date**

---

## 🧹 Data Cleaning Process

Performed in **Power Query**:

1. **Removed Duplicates:**  
   Ensured unique and valid employee records.

2. **Added Conditional Columns:**  
   - Mapped `Education` levels (1–5) → `"Below College"` to `"Doctor"`.
   - Grouped `Age` into ranges (`18–25`, `26–38`, etc.).
   - Converted `Attrition` → `"Still Working"` / `"Left The Company"`.

3. **Custom Columns:**
   - `EndDate` & `InvalidReview` to identify and filter faulty data.

4. **Standardization:**
   - Replaced inconsistent values.
   - Transformed column types using `Table.TransformColumnTypes`.

---

## 🧠 Data Modeling

Implemented a **star schema** model with fact and dimension tables.

### Fact Tables:
- `FactEmployee`: Tracks attributes like Department, Travel, Education.
- `FactPerformanceRating`: Contains ratings and review dates.

### Dimension Tables:
- `DimDate`: Time hierarchy (DayName, DayNumber, etc.).
- `DimSatisfactionLevel` / `DimRatingLevel`: Satisfaction scales.

> Relationships were established using `EmployeeID` and temporal keys to support slicing data across different perspectives.

---

## 📊 Dashboard Features

The Power BI dashboard was divided into **4 key pages**:

1. **Overview:**
   - Workforce size, education levels, department distribution, general stats.

2. **Demographics:**
   - Age, gender, marital status, ethnicity, and salary distribution.

3. **Performance Tracker:**
   - Individual employee satisfaction and performance over time.

4. **Attrition Insights:**
   - Attrition rate, inactive count, hire/tenure date, travel frequency, and overtime.

Each visual enabled drill-through and filtering for deeper exploration.

---

## 🧮 DAX Usage

Custom metrics were calculated using **DAX**, including:
- Attrition rate by department and job role.
- Time intelligence metrics: Year, Month, Day from `ReviewDate`.
- Measures to track satisfaction averages and performance over time.

---

## 💡 Key Insights & Recommendations

1. **Target Age Group 18–30:**  
   Introduce mentorship programs to retain younger employees.

2. **Ethnicity Pay Gap:**  
   Perform salary audits and implement transparent pay scales.

3. **New Hire Support:**  
   Improve onboarding and offer early-career mentorship.

4. **Overtime Risks:**  
   Redistribute workload or hire to ease excessive hours.

5. **Travel Frequency:**  
   Balance business travel assignments across staff.

---

## 📈 Impact & Lessons Learned

- **Strategic Value:** Helped HR visualize critical metrics and formulate retention strategies.
- **Team Collaboration:** Effective use of cloud tools, regular check-ins, and defined task ownership led to successful project execution.
- **Challenges Overcome:** Initial data complexity was addressed through iterative cleaning and modeling.

---

## 🏁 Conclusion

This BI project provided the organization with a **scalable, interactive, and insightful dashboard** that transformed raw HR data into **actionable decisions** for reducing attrition, enhancing satisfaction, and driving organizational growth.


