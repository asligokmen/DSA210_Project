# Multivariate Analysis of Factors Influencing Student Exam Performance

## Research Question
How do sleep duration, study hours, stress level, and previous academic performance collectively influence students’ exam scores?

## Motivation
Student academic success is shaped by multiple behavioral and lifestyle factors. While sleep duration affects cognitive performance, variables such as stress level, study habits, class attendance, and previous exam experience also play major roles. This project aims to analyze how these factors *together* influence exam performance. Understanding these relationships helps students make better decisions regarding time management, sleep schedules, stress control, and study strategies.

## Data Sources

### Student Exam Scores Dataset
- File: `student_exam_scores.csv`
- Link: https://www.kaggle.com/datasets/mirzayasirabdullah07/student-exam-scores-dataset  
- Variables:
  - student_id  
  - hours_studied  
  - sleep_hours  
  - attendance_percent  
  - previous_scores  
  - exam_score  

### Student Performance Score Dataset
- File: `SrudentPerformanceScore.csv`
- Link: https://www.kaggle.com/datasets/mustafamaher2520/student-performance-data  
- Variables:
  - Student_ID  
  - Sleep_Hours  
  - Study_Hours  
  - Stress_Level  
  - Previous_Exam_Scores  

Both datasets are merged using `student_id`.

## 4. Features Used
- Sleep Hours  
- Study Hours  
- Stress Level  
- Attendance Percent  
- Previous Scores  
- Exam Score (dependent variable)

## 5. Methodology

### Data Cleaning
- Standardized column names  
- Removed missing or inconsistent entries  
- Cleaned student ID fields  
- Merged datasets using inner join  
- Created sleep categories (<6h, 6–8h, >8h)

### Exploratory Data Analysis (EDA)
- Descriptive statistics  
- Histograms for key variables  
- Scatter plots  
- Correlation matrix  
- Boxplots by sleep category  

### Hypothesis Testing
- Pearson correlation tests  
- ANOVA across sleep categories  
- Simple regression (Sleep → Exam Score)  
- Multiple regression (Sleep + Study + Stress + Previous Scores → Exam Score)

## Expected Outcome
It is expected that multiple academic and lifestyle factors—including sleep habits, study hours, stress level, and prior performance—collectively influence exam outcomes. Regression analysis will help identify which factors act as the strongest predictors of exam performance.

## Tools
- Python  
- pandas  
- seaborn  
- matplotlib  
- statsmodels  
- scipy  
- Jupyter Notebook / Google Colab
- 
## 30 November Deliverables
- Raw datasets uploaded under /data  
- Full EDA performed in analysis.ipynb  
- Data cleaning steps included  
- Hypothesis testing (correlation, ANOVA, regression) completed  
- Visualizations included (histograms, scatter plots, heatmap, boxplots)
- 
## 02 January Deliverables 
- Applied supervised machine learning methods to predict student performance.
- Analyzed the two datasets separately.
- Used Linear Regression and Random Forest Regression models.
- Split datasets into training 80% and test 20% sets.
- Applied feature scaling using StandardScaler where required.
- Evaluated models using R^2 score and Mean Squared Error.

## Author
Prepared by: Aslı Gökmen  
Course: DSA210 – Introduction to Data Science  
Term: Fall 2025–2026
