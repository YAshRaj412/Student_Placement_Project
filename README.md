

# Student Placement Data Analysis

## Project Overview

This project performs an Exploratory Data Analysis (EDA) on student performance metrics to identify factors influencing job placement and salary packages (CTC). Using a dataset of 150 students, the analysis explores the relationship between assignment completion, communication skills, content scores, and final career outcomes across different technical courses.

---

## Dataset Description

The analysis is performed on `student_placement_data.csv` which includes:

* **Student Profile:** ID, Name, and Course (Data Analytics, Python DA, Full Stack Web Dev).
* **Performance Metrics:** Assignment Completion %, Content Score Average, and Communication Skills (rated out of 10).
* **Placement Outcomes:** Placement status (Yes/No) and CTC in LPA (Lakhs Per Annum).

---

## Key Insights from the Analysis

### 1. Placement Factors

Analysis shows that students who were successfully placed had significantly higher **Content Score Averages** (~73.18) compared to those who were not (~62.22). Interestingly, the average **Assignment Completion %** remained relatively consistent (approx. 71-72%) regardless of placement status.

### 2. Communication Skills

The dataset shows a diverse range of communication abilities:

* **30 students** achieved a perfect 10/10 score.
* Placed students had a higher average communication score (6.83) compared to unplaced students (6.07).

### 3. Salary Analysis by Course

The average CTC varies by specialized track:
| Course | Average CTC (LPA) |
| :--- | :--- |
| **Python DA** | 6.47 |
| **Full Stack Web Dev** | 6.18 |
| **Data Analytics** | 5.99 |

---

## Implementation Details

### Requirements

To run this notebook, you need the following libraries:

```bash
pip install pandas

```

### Core Operations Performed

1. **Data Cleaning:** Checked for missing values in CTC and identified non-null counts across 9 columns.
2. **Descriptive Statistics:** Generated mean, standard deviation, and quartiles for numerical features.
3. **Grouping & Aggregation:** Segmented data by `Course` and `Placed` status to find average performance metrics.
4. **Correlation:** Analyzed the relationship between `Assignment_Completion_%` and `CTC_LPA`, finding a very weak negative correlation (-0.02).
5. **Sorting:** Identified top performers based on assignment completion.

---

## How to Use

1. **Clone the Repository:**
```bash
git clone https://github.com/YAshRaj412/Student_Placement_Project.git

```


2. **Run the Notebook:** Open `pandas_student_placement_practice.ipynb` in Jupyter Notebook or Google Colab to view the step-by-step analysis.

---
