## 📌 Project 1: Basic Level – Student Performance Dashboard

An introductory-level dashboard built for visualizing general trends in academic performance and student metrics.

<img width="1025" alt="Screenshot 2025-04-13 at 11 01 38 AM" src="https://github.com/user-attachments/assets/a7948120-10f4-4419-aa5a-df146e7d3061" /># 📊 Student Performance Dashboard (Power BI)



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

DAX
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

![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/422631c1-c64a-4354-8540-1bf9aa88fba6)


## 📌 Project 2: Intermediate Level – Advanced Student Analytics

<img width="960" alt="Screenshot 2025-04-13 at 1 55 17 PM" src="https://github.com/user-attachments/assets/98f33119-9dc4-4004-a427-cb464139c824" />



This intermediate-level Power BI dashboard builds upon the basic version by offering in-depth analytics related to institutional KPIs, financial metrics, and academic insights.

---

### ✅ Key Highlights

- 🎓 **Total Students**: 6,200  
- 📚 **Total Courses**: 50  
- ✅ **Total Passed**: 5,604 students (**90.4%**)  
- ❌ **Total Failed**: 596 students (**9.6%**)

---

### 📊 Visual Components

- **KPI Cards** for students, courses, passed, and failed counts
- **Treemap** showing monthly book return volumes
- **Bar Chart** for Payment Method trends over time
- **Country vs Department Matrix** with totals for Arts, Commerce, Engineering, and Science
- **Time Series with Forecast** for enrollment trends using DateTable

---

### 💡 Insights Derived

- Most students passed, with a high academic success rate across departments.
- Online Payments dominate financial transactions in recent years.

- Library data shows active usage with cyclical return patterns.
- Enrollment trends are flattening, with minor future decline expected—calling for student engagement initiatives.
- Countries like **El Salvador**, **Ireland**, and **Germany** show strong representation across multiple academic streams.

