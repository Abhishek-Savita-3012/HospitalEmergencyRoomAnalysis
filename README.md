# Hospital Emergency Room Dashboard

## 📌 Project Overview

The **Hospital Emergency Room Dashboard** is an Excel-based data analysis project designed to analyze emergency room patient data and provide useful insights for hospital management.

This dashboard helps track patient flow, waiting time, satisfaction score, admission status, gender distribution, age group distribution, department referrals, and daily patient trends.

The main purpose of this project is to improve emergency room efficiency and support better decision-making through data visualization.

---

## 🎯 Project Objective

The objective of this project is to create an interactive dashboard that helps analyze hospital emergency room performance.

The dashboard focuses on:

- Total number of patients
- Average patient wait time
- Patient satisfaction score
- Admission and non-admission status
- Patients attended within time
- Delayed patients
- Gender-wise patient distribution
- Age group-wise patient distribution
- Department referral analysis
- Daily patient trend analysis

---

## 🛠️ Tools and Technologies Used

- Microsoft Excel
- Power Query
- Power Pivot
- DAX
- Pivot Tables
- Pivot Charts
- Slicers
- Data Cleaning
- Data Modeling
- Dashboard Design
- Data Visualization

---

## 📁 Project Files

| File Name | Description |
|---|---|
| `Hospital_Emergency_Room_Data.xlsx` | Raw hospital emergency room dataset |
| `ExcelProjectHospitalPatientAnalysis.xlsx` | Final Excel dashboard file |
| `Hospital_Emergency_Room_PPT.pptx` | Project presentation |
| `HospitalEmergencyRoomFinalDashboard.png` | Final dashboard screenshot |
| `AverageWaitingTimeSparkline.png` | Daily average wait time trend |
| `PatientSatisfactionSparkline.png` | Daily patient satisfaction trend |
| `PatientsPerDaySparkline.png` | Daily patient count trend |

---

## 📊 Key Performance Indicators

| KPI | Value |
|---|---:|
| Number of Patients | 442 |
| Average Wait Time | 35.60 minutes |
| Patient Satisfaction Score | 4.8 |
| Patients Attended On Time | 40% |
| Delayed Patients | 60% |
| Female Patients | 50% |
| Male Patients | 50% |

---

## 📈 Dashboard Features

- Monthly emergency room report
- Year selection filter for 2023 and 2024
- Month-wise slicer
- Number of patients KPI card
- Average wait time KPI card
- Patient satisfaction score KPI card
- Admission status analysis
- Age group-wise patient analysis
- Timeliness analysis
- Gender-wise patient analysis
- Department referral analysis
- Daily trend sparklines

---

## 🔍 Business Requirements

The dashboard was created based on the following business requirements:

1. Count the total number of patients visiting the emergency room.
2. Track the average waiting time of patients.
3. Analyze the patient satisfaction score.
4. Compare admitted and not admitted patients.
5. Identify patients attended within time and delayed patients.
6. Analyze patients by gender.
7. Group patients by age category.
8. Identify department referrals.
9. Track daily patient trends using sparklines.

---

## 📌 Key Insights

### 1. Number of Patients

The dashboard shows a total of **442 patients** for the selected month.

Daily patient trends are displayed using an area sparkline to identify busy days and patient flow patterns.

---

### 2. Average Wait Time

The average patient wait time is:

**35.60 minutes**

This means patients wait around 36 minutes on average before being attended by a medical professional.

---

### 3. Patient Satisfaction Score

The average patient satisfaction score is:

**4.8**

This score helps evaluate the quality of emergency room service and patient experience.

---

### 4. Admission Status

| Admission Status | Number of Patients | Percentage |
|---|---:|---:|
| Not Admitted | 304 | 50.84% |
| Admitted | 294 | 49.16% |

The admission status is almost balanced, with slightly more patients not admitted than admitted.

---

### 5. Timeliness Analysis

| Status | Percentage |
|---|---:|
| Delay | 60% |
| On Time | 40% |

Most patients experienced delay, which shows that wait time management needs improvement.

---

### 6. Gender-wise Analysis

| Gender | Percentage |
|---|---:|
| Female | 50% |
| Male | 50% |

The patient distribution by gender is equal.

---

### 7. Age Group Analysis

| Age Group | Number of Patients |
|---|---:|
| 0-09 | 55 |
| 10-19 | 59 |
| 20-29 | 65 |
| 30-39 | 55 |
| 40-49 | 50 |
| 50-59 | 60 |
| 60-69 | 54 |
| 70-79 | 44 |

The highest number of patients belong to the **20-29 age group**, followed by **50-59** and **10-19**.

---

### 8. Department Referral Analysis

| Department Referral | Number of Patients |
|---|---:|
| None | 259 |
| General Practice | 91 |
| Orthopedics | 50 |
| Physiotherapy | 17 |
| Cardiology | 12 |
| Gastroenterology | 6 |
| Neurology | 5 |
| Renal | 2 |

Most patients were not referred to any department. Among referred patients, **General Practice** received the highest number of referrals.

---

## 🧹 Data Preparation Steps

The project followed these steps:

1. Business requirement gathering
2. Understanding the dataset
3. Importing data using Power Query
4. Data cleaning and data quality check
5. Creating a calendar table
6. Data modeling using Power Pivot
7. Adding required columns using DAX
8. Creating pivot tables
9. Creating pivot charts
10. Dashboard layout design
11. Chart formatting
12. Final dashboard development
13. Insight generation

---

## 🧾 Calendar Table Formula

```powerquery
= List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))
```

---

## 🧮 DAX Formulas Used

### Age Group Formula

```DAX
=IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))
```

### Patient Attend Status Formula

```DAX
=IF([Patient Waittime]<30,"Within Time","Delay")
```

---

## 💡 Recommendations

- Reduce patient waiting time by improving staff allocation during busy days.
- Focus on reducing delayed patients because 60% of patients are not attended within time.
- Monitor daily patient trends to identify high-pressure days.
- Improve emergency room workflow to increase patient satisfaction.
- Analyze departments with high referrals to allocate resources properly.
- Use age group trends to plan healthcare services better.
- Track satisfaction score regularly and compare it with waiting time trends.
- Improve scheduling and resource planning during high patient volume days.

---

## 📚 Skills Demonstrated

- Data Cleaning
- Power Query
- Power Pivot
- DAX Calculations
- Data Modeling
- Pivot Table Analysis
- Pivot Chart Creation
- Dashboard Creation
- KPI Reporting
- Healthcare Data Analysis
- Data Visualization
- Business Insight Generation

---

## 🏁 Conclusion

This project successfully analyzes hospital emergency room data using Microsoft Excel, Power Query, Power Pivot, and DAX.

The dashboard provides important insights into patient count, average waiting time, satisfaction score, admission status, gender distribution, age group distribution, timeliness, and department referrals.

The analysis shows that the emergency room has balanced gender distribution and strong patient flow, but wait time and delayed patients need improvement.

These insights can help hospital management improve emergency room efficiency, reduce patient waiting time, and enhance overall patient care.
