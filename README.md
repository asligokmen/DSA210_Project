# The Relationship Between Sleep Duration and Exam Performance Among Students

# Research Question
Do students who sleep longer hours achieve higher exam scores on average?

# Motivation
Students' cognitive abilities, including memory, focus, and learning effectiveness, are greatly impacted by sleep. Many students forgo sleep during exam times because they think it would help them perform better. However, research indicates that sleep deprivation may hinder concentration and lower exam scores.

This project's goal is to determine whether students who get more sleep before tests typically do better. The initiative intends to shed light on how lifestyle choices affect academic performance by examining sleep patterns in conjunction with test scores.

Teachers and students can make better decisions about sleep management and study schedules if they are aware of this relationship.

# Data Sources

Student Exam Scores Dataset
File: student_exam_scores.csv
Description: Contains students’ exam performance across different subjects and exams.
Key Variables (examples):
Student_ID: unique identifier for each student
Exam_Score: score obtained in each exam
Subject: name of the subject or exam type
Study_Hours: number of hours studied before the exam

Student Performance Score Dataset
File: SrudentPerformanceScore.csv
Description: Provides information about each student’s sleep duration and related lifestyle habits.
Key Variables (examples):
Student_ID: student identifier (to merge with exam dataset)
Sleep_Hours: average daily sleep duration
Performance_Score: overall academic performance indicator
Stress_Level: stress rating or level reported by the student
The datasets will be merged using the Student_ID column so that each student’s exam results can be analyzed together with their sleep information.

# Methodology
---
**Data Cleaning**
Remove missing or inconsistent entries (e.g., students without exam or sleep data).
Standardize student identifiers and ensure matching between datasets.
Convert categorical variables into numeric form if necessary.
---
**Data Integration**
Merge both datasets on Student_ID.
Create a combined dataset that includes each student’s exam score, study hours, and sleep duration.
---
**Data Analysis**
Calculate each student’s average exam score.
Explore how Sleep_Hours correlates with Exam_Score.
Compare mean exam scores across different sleep ranges (e.g., <6h, 6–8h, >8h).
Use correlation analysis and regression modeling to test if longer sleep is associated with higher exam performance.
---
**Visualization**
Scatter plots: Sleep hours vs Exam scores
Box plots: Exam scores grouped by sleep duration categories
Correlation heatmap: Sleep hours, study hours, and exam scores
