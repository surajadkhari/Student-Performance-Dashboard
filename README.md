
Welcome to the **Student Performance Dashboard** project – an interactive Power BI report designed to visualize and analyze student academic and transactional data for better decision-making.

---

<img width="1025" alt="Screenshot 2025-04-13 at 11 01 38 AM" src="https://github.com/user-attachments/assets/a7948120-10f4-4419-aa5a-df146e7d3061" /># 📊 Student Performance Dashboard (Power BI)

---

## 🔍 Project Overview

This dashboard leverages multiple tables including:

- `student_data`
- `exams_data`
- `payments_data`
- `library_data`
- `DateTable` (custom-built using DAX)

**Main Objective:**  
To provide actionable insights into:
- Student academic performance  
- Enrollment trends  
- Payment behaviors  
- Country & stream-wise distributions  

---

## 📌 Key Insights

- 🧮 Grade Breakdown (A, B, C)
- 🌍 Student Country vs. Academic Stream matrix
- 🗓️ Student enrollment trend with forecast
- 💳 Payment method comparison (Cash, Online, Credit, Transfer)
- 📆 Time-based analysis using a custom Date Table

---

## 🧠 Time Intelligence Table (DAX)

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


🧩 This DateTable enables:

Yearly & monthly trend analysis

Slicer filtering for different time frames

Forecasting based on historical data

✨ Tools & Technologies Used
Power BI – Data modeling, visualizations, DAX calculations

DAX – Measures and calculated columns

![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/422631c1-c64a-4354-8540-1bf9aa88fba6)

