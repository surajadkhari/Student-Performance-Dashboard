# 📊 Student Performance Dashboard (Power BI)

Welcome to the **Student Performance Dashboard** project, where I've designed an interactive Power BI report that provides actionable insights into student data, grades, and payment methods.

---

## 🔍 Project Overview

This dashboard was built using multiple student-related datasets including:

- `student_data`  
- `exams_data`  
- `payments_data`  
- `library_data`  
- A custom `DateTable` for time intelligence

**Objective:**  
To explore and visualize key metrics such as student performance by grade, yearly enrollment trends, payment methods, and breakdown by country and department.

---

## 📌 Key Features

- 📅 **Time Intelligence**: Count of students by year using a custom `DateTable`
- 📈 **Trend Analysis**: Yearly student ID trends with forecasting
- 🧮 **Grade Insights**: Distribution of students by grade (A, B, C)
- 🌍 **Country & Stream**: Student distribution across countries and academic streams
- 💳 **Payments Analysis**: Breakdown of payment methods used by students

---

## 🧠 Time Intelligence Table

I created a dynamic `DateTable` using DAX to support advanced date filtering and time-based analysis:

```DAX
DateTable = 
ADDCOLUMNS(
    CALENDAR(DATE(2010, 1, 1), DATE(2030, 12, 31)),
    "Year", YEAR([Date]),
    "Month", MONTH([Date]),
    "Month Name", FORMAT([Date], "MMMM"),
    "Quarter", QUARTER([Date]),
    "Day", DAY([Date]),
    "Weekday", WEEKDAY([Date]),
    "Weekday Name", FORMAT([Date], "dddd"),
    "Year-Month", FORMAT([Date], "YYYY-MM")

)

![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/50f02f6e-079e-4d47-b7ac-c269672367de)
