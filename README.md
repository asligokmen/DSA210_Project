# Multivariate Analysis of Factors Influencing Student Exam Performance

## Project Overview
This project investigates academic and lifestyle factors influencing students’ exam performance from a multivariate perspective. The analysis focuses on how sleep duration, study hours, stress level, attendance rate, and previous academic performance jointly affect exam scores.

The project was prepared as a term project for DSA210 – Introduction to Data Science. According to the course guidelines, a separate PDF report is not required. Instead, this README summarizes the project motivation, data sources, methodology, findings, and limitations, while detailed analyses, numerical results, and code implementations are provided in the accompanying Jupyter notebooks.

## Research Question
How do sleep duration, study hours, stress level, attendance, and previous academic performance collectively influence students’ exam scores?

Rather than examining each factor in isolation, this project aims to understand how these variables interact and jointly contribute to academic outcomes.

## Motivation
Student academic success is shaped by a combination of behavioral, cognitive, and lifestyle-related factors. While prior research often examines variables such as sleep or study time independently, real-world performance is influenced by the interaction of multiple factors.

This project aims to:
- Provide data-driven insights into how academic and lifestyle variables jointly influence exam performance
- Help students make more informed decisions about time management, sleep habits, and stress control
- Demonstrate the use of multivariate statistical analysis and machine learning techniques in an educational context

## Data Sources
Two publicly available Kaggle datasets were used in this project.

Student Exam Scores Dataset:
File: student_exam_scores.csv  
Source: https://www.kaggle.com/datasets/mirzayasirabdullah07/student-exam-scores-dataset  
Variables:
- student_id
- hours_studied
- sleep_hours
- attendance_percent
- previous_scores
- exam_score

Student Performance Score Dataset:
File: SrudentPerformanceScore.csv  
Source: https://www.kaggle.com/datasets/mustafamaher2520/student-performance-data  
Variables:
- Student_ID
- Sleep_Hours
- Study_Hours
- Stress_Level
- Previous_Exam_Scores

The two datasets were merged using the student_id field after preprocessing and standardization.

## Features Used
- Sleep Hours
- Study Hours
- Stress Level
- Attendance Percent
- Previous Scores
- Exam Score (dependent variable)

## Methodology

Data Cleaning and Preprocessing:
- Standardized column names across datasets
- Removed missing and inconsistent observations
- Cleaned and aligned student ID fields
- Merged datasets using an inner join
- Categorized sleep duration into < 6 hours, 6–8 hours, and > 8 hours

Exploratory Data Analysis (EDA):
- Descriptive statistics for all variables
- Distribution analysis using histograms
- Scatter plot analysis of key relationships
- Correlation matrix
- Boxplots comparing exam scores across sleep categories

Statistical Analysis and Hypothesis Testing:
- Pearson correlation tests
- ANOVA across sleep duration categories
- Simple linear regression (Sleep → Exam Score)
- Multiple linear regression (Sleep, Study, Stress, Previous Scores → Exam Score)

## Machine Learning Extension
In addition to statistical analyses, supervised machine learning models were applied to predict student exam performance.

Models used:
- Linear Regression
- Random Forest Regression

Modeling pipeline:
- Each dataset analyzed separately
- Train–test split: 80% training and 20% testing
- Feature scaling using StandardScaler where required
- Model evaluation using R² Score and Mean Squared Error (MSE)

## Summary of Findings
Overall results indicate that:
- Previous academic performance is one of the strongest predictors of exam scores
- Sleep duration and study hours have meaningful but limited standalone effects
- Higher stress levels are generally associated with lower performance
- Multivariate regression and machine learning models provide stronger explanatory power than single-variable analyses

Detailed numerical results, tables, and visualizations are available in the project notebooks.

## Limitations
- The datasets are secondary or synthetic and may not fully reflect real-world student populations
- Individual learning styles and course difficulty levels are not captured
- Stress level is based on self-reported measures
- No temporal or user-history modeling was applied

## Project Structure
data/
- student_exam_scores.csv
- SrudentPerformanceScore.csv

analysis.ipynb  
ml_models.ipynb  
README.md

## Tools and Technologies
- Python
- pandas
- matplotlib
- seaborn
- scipy
- statsmodels
- scikit-learn
- Jupyter Notebook / Google Colab

## Author
Prepared by: Aslı Gökmen  
Course: DSA210 – Introduction to Data Science  
Term: Fall 2025–2026
