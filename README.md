# Module 4 Challenge (JB Trahin): School District Analysis
Module 4 challenge on performing a school district analysis using Python, Pandas, NumPy, Anaconda and Jupyter Notebook.

## Project Overview
We are completing a school district analysis to help plan budget allocation for the following year. 

We learned that the grades of the ninth graders at Thomas High School have been changed. While administrators do not know the full extent of this academic dishonesty, they want to uphold the standards of state testing and have turned to you for help.

We have decided that the best approach is to:

- Remove all the math and reading scores of the ninth graders at Thomas High School.
- Keep all other data associated with the ninth-grade students and Thomas High School intact.

In this project, our final Python script will need to be able to deliver the following information when ran on top of a provided xls spreadsheets: 

1. A high-level snapshot of the district's key metrics, presented in a table format
2. An overview of the key metrics for each school, presented in a table format
3. Tables presenting each of the following metrics:
    - Top 5 and bottom 5 performing schools, based on the overall passing rate
    - The average math score received by students in each grade level at each school
    - The average reading score received by students in each grade level at each school
    - School performance based on the budget per student
    - School performance based on the school size 
    - School performance based on the type of school

We will run our script on the intial dataset we were provided first, before removing all the reading math scores of the affected population and running the script a second time. We'll then answer the following questions by comparing the two results across all metrics:
1. How is the district summary affected?
2. How is the school summary affected?
3. How does removing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
4. How does removing the ninth grade scores affect the following:
    - Math and Reading Scores by Grade
    - Scores by School Spending
    - Scores by School Size
    - Scores by School Type

## Resources
- Data Source: schools_complete.csv, students_complete.csv
- Software: Python 3.6.1, Pandas 0.25.1, NumPy 1.17.2, Anaconda 2019.10, Conda 4.7.12, Jupyter Notebook 6.0.1

## Summary
The analysis of the school district data shows that:
- There is 461 students that were affected by the grade change and removed from the calculations.

- Here is how the district summary was affected:
    - the number of total schools remained the same (15).
    - the number of total students went from 39,170 down to 38,709 (-1.2%).
    - the total budget remained the same ($24,649,428).
    - the average math score went from 79 down to 78.9 (-0.1%).
    - the average reading score remained the same (81.9).
    - the % of students passing math remained the same (75%).
    - the % of students passing reading remained the same (86%).
    - the overall passing % of students passing both remained the same (65%).

- Here is how the school summary is affected:
    - the only school in the school summary where we observe a change in the outcome is Thomas High School

- Here is how removing the ninth graders’ math and reading scores affected Thomas High School’s performance, relative to the other schools:
    - Thomas High School now had the highest per student budget ($888.53).
    - Thomas High School's average math score went from 83.41 down to 83.35 (-0.07%).
    - Thomas High School's average reading score went from 83.85 up to 83.90 (+0.06%).
    - Thomas High School's passing math % went from 93.27% down to 93.19% (-0.09%).
    - Thomas High School's passing reading % went from 97.31% down to 97.02% (-0.3%).
    - Thomas High School's overall % for passing both went from 90.95% down to 90.63% (-0.4%).
We can say that the biggest change is for the per student budget. Cutting the total number of students without readjusting the budget creates that unbalance.

- Here is how removing the ninth grade scores affect Math and Reading Scores by Grade:
    - We notice a NaN value for math and reading score for students in the 9th grade at Thomas High School.

- Here is how removing the ninth grade scores affect Scores by School Spending:
    - We notice a change in the $630-644 spending per student range:
        - the % of students passing math went from 73 down to 67 (-8%).
        - the % of students passing reading went from 84 down to 80 (-5%).
        - the overall passing % of students passing both went from 63 down to 53 (-16%).

- Here is how removing the ninth grade scores affect Scores by School Size:
    - We don't notice any significant changes.

- Here is how removing the ninth grade scores affect Scores by School Type:
    - We don't notice any significant changes.


  
