# OVERVIEW

This project showcases a comprehensive Power BI dashboard developed for **LearnSphere**, an online learning platform. 

I led the end-to-end design of a reporting solution that delivers actionable insights across **student lifecycle analytics**, **course performance**, **instructor productivity**, and **institutional financials**.

The goal was to simulate a real-world business case, where decision-makers at an edtech firm need data-driven intelligence to improve academic outcomes, optimize instructor allocation, and ensure sustainable revenue flow.


## Project Objectives

The project was built to address the following business objectives

- What are the **enrollment trends** across months and departments
- What are the students that are *active*,*dropped* or *graduated* and whats their academic performance
- Which **instructors** are driving student success and how do their ratings compare?
- Which courses are *in-demand* and how does course difficulty impact performance?
- How much revenue is being generated? and what are the trends in **pending payments** and **scholarship distribution**


## Analytical Approach

### 1. **Student Analytics**
- Created a dynamic segmentation of students status(Active, Dropped, Graduated)
- Analyzed **attendance rate vs GPA**, department performance of students etc
- Tracked **monthly enrollment trends** to identify seasonal engagement patterns

**Students Analytics**

![Student Page](images/Student_Page.png)

### 2. **Course Performance Analysis**
- Evaluated course difficulty levels(Beginner, Intermediate,Advanced)
- Measured student success rates by course
- Ranked courses by popularity and average GPA

**Course Perforance Analytics**

![Course Page](images/Courses_Page.png)

### 3. **Instructor Performance Analytics**
- Assessed instructor workload: students per instructor
- Compared average credit load with performance ratings
- Identified top rated and low-performing instructors to informing retention and training strategies

**Instructor Performance Analytics**

![Instructor Page](images/Instructor_Page.png)

### 4. **Financial Analytics**
- Broke down students on **tuition vs scholarship** across departments
- Monitored payment status
- Highlighted key revenue contributors

**Financial Analytics**

![Financials Page](images/Financials_Page.png)



## Data Model Overview

The Power BI data model was built using **Star Schema** principles for performance and scalability:

- **Fact Tables**: Student Table
- **Dimension Tables**: Students, Instructors, Courses, Financials.


Below is the image of the Data Model

![Data Model](images/Data_Model.png)



> All data was cleansed and transformed using **Power Query**. Calculations and KPIs were built using **DAX** to ensure optimized performance and modularity.



## Dashboard Highlights

| Area | Description |
|------|-------------|
| **Students Overview** | Live stats on total students, attendance rate, grade distribution |
| **Course Performance** | Comparative charts for difficulty level, GPA by course, and dropout patterns |
| **Instructor Insights** | Ratings, satisfaction scores, experience distribution, student load |
| **Financials** | Revenue funnel, tuition vs scholarship, overdue payment trends |

### Drillthrough Pages

Drillthrough pages allow stakeholders to right-click and explore **individual student records** or **detailed financial breakdowns**.

#### Student Performance Drillthrough
- View student-level metrics: SAT scores, midterm/final exams, attendance, and academic standing
- Designed for academic advisors and instructors to monitor student success

**Student Drillthrough**

![Student Drillthrough](images/Drillthrough_Page1.png)


#### Financial Status Drillthrough
- Displays full payment record: tuition fees, scholarships, overdue amounts
- Helps the finance team target students with payment issues

**Financial Drillthrough**


![Financial Drillthrough](images/Drillthrough_Pagge2.png)



## Tools & Technologies

| Tool | Use |
|------|-----|
| **Power BI Desktop** | Data modeling, dashboard creation |
| **Power Query** | Data transformation and cleaning |
| **DAX** | Business logic and KPIs |
| **Star Schema Modeling** | Scalable, optimized data architecture |



## Key Business Insights

Here are some key takeaways derived from the dashboard:

- **Melissa Jackson** has the highest student load (503) with a high performance rating (4.98), suggesting scalable teaching efficiency.
- The **Data Science** and **Cybersecurity** departments each contribute over 33% to LearnSphere’s total revenue.
- **Over 25% of students** are flagged for intervention based on attendance, payment status, or poor grades.
- **$17M in pending tuition fees** poses a major risk to cash flow; most overdue payments are concentrated in the Computer Science and Psychology majors.


## Future Enhancements

- Add **Row-Level Security (RLS)** for department heads
- Enable **data refresh via Power BI Service**