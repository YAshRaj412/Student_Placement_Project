# Student_Placement_Project

📝 Project Overview
I built this exploratory data analysis (EDA) project using Python and the Pandas library. The project loads, inspects, and analyzes a dataset of 150 student records (student_placement_data.csv) to uncover insights and trends related to student placements.

I began by loading the data and using functions like .info() and .describe() to understand its structure, identify data types, and find missing values (noting 41 null values in the CTC_LPA column).

📊 Key Questions & Analyses Performed
My analysis successfully answers several key questions about the placement data:

What is the average CTC for each course?

I grouped the data by Course and calculated the mean CTC_LPA for each, finding that "Python DA" has the highest average CTC (6.47 LPA), followed by "Full Stack Web Dev" (6.18 LPA), and "Data Analytics" (5.99 LPA).

How do placed vs. unplaced students compare?

I grouped the data by Placed status and found that placed students have a notably higher average Content Score (73.18 vs. 62.22) and Communication Skill (6.83 vs. 6.07) than unplaced students.

What is the placement rate for each course?

I used a groupby() operation followed by .size().unstack() to create a pivot table showing the exact count of "Yes" (Placed) vs. "No" (Not Placed) students for each course.

Who are the top-performing students?

I sorted the entire dataset by Assignment_Completion_% in descending order to identify and display the top 10 students.

Is there a correlation between assignment completion and salary?

I used the .corr() method to find the correlation between Assignment_Completion_% and CTC_LPA, discovering a very weak negative correlation (-0.02).

💻 Technologies Used
Python

Pandas (for loading, cleaning, grouping, and analyzing the data)

Jupyter Notebook (as the environment for the analysis)
