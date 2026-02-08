## 🎯 What I Did in This Project

In this project, I explained real analytical questions related to **student exam performance**, including:

* How to calculate **actual marks** when negative marking is applied
* Which students **passed** and which **failed**
* Who are the **top 5 performers** in each exam
* Whether students are **improving or declining** over time
* How these trends look when **visualized using charts**

---

## 🧰 Tools & Technologies Used

| Category        | Tools                                        |
| --------------- | -------------------------------------------- |
| Environment     | Google Colab (Python 3)                      |
| Database        | SQLite (in-memory)                           |
| Data Processing | pandas, NumPy                                |
| Visualization   | matplotlib, seaborn                          |
| SQL Features    | CTE, JOIN, CASE, RANK(), LAG(), PARTITION BY |

---

## 📁 Dataset Overview

This project uses **two CSV files**.

### 1️⃣ `exams.csv`

| Column                    | Description                           |
| ------------------------- | ------------------------------------- |
| exam_id                   | Unique ID for each exam               |
| exam_name                 | Name of the exam                      |
| each_ques_mark            | Marks awarded for each correct answer |
| per_ques_negative_marking | Marks deducted for each wrong answer  |
| pass_mark                 | Minimum marks required to pass        |

---

### 2️⃣ `exam_sessions.csv`

| Column                | Description                       |
| --------------------- | --------------------------------- |
| session_id            | Unique ID for each exam attempt   |
| user_id               | Student ID                        |
| exam_id               | Exam taken by the student         |
| total_correct_answers | Number of correct answers         |
| total_false_answers   | Number of wrong answers           |
| user_exam_starts_at   | Date and time of the exam attempt |

---

## 🔬 How I Did It (Step by Step)

### Step 1: Setup and Load Data

* Loaded the CSV files using **pandas**
* Converted date columns into proper **datetime format**
* Created an **in-memory SQLite database**
* Stored pandas DataFrames as SQL tables

This approach allowed me to run **real SQL queries directly on CSV data** while still using Python for processing and visualization.
