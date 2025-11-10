# Healthcare Data Analysis Power BI Project

# 🏥 Healthcare Analytics Dashboard – Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-blue?style=for-the-badge)
![Data](https://img.shields.io/badge/Data-Analysis-green?style=for-the-badge)

---

## 📊 Overview
This **Healthcare Analytics Dashboard** enables hospitals and clinics to make data-driven decisions.  
It provides insights into patient demographics, hospital performance, and disease patterns.

---

## 🧮 Key Measures (DAX)
```DAX
Total Patients = COUNT(Patient_Data[PatientID])
Average Stay (Days) = AVERAGE(Patient_Data[LengthOfStay])
Total Revenue = SUM(Patient_Data[Revenue])
Readmission Rate = DIVIDE(
    CALCULATE(COUNT(Patient_Data[PatientID]), Patient_Data[Readmitted] = "Yes"),
    [Total Patients]
)
