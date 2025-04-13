# 📊 Student Performance Dashboard (Power BI)

Welcome to the **Student Performance Dashboard** project – an interactive Power BI report designed to visualize and analyze student academic and transactional data for better decision-making.

---

## 🎥 Dashboard Preview

![Student Performance Dashboard Demo](./Untitled%20video%20-%20Made%20with%20Clipchamp.gif)

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
