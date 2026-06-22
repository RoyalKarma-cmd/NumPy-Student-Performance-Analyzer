# 📊 NumPy Student Performance Analyzer

A beginner-friendly Data Analytics project built using **NumPy** to analyze student performance across multiple subjects using a **2D Array (Matrix)**.

This project demonstrates how to perform statistical analysis on student marks, calculate student-wise and subject-wise averages, and identify the class topper using NumPy.

---

## 🚀 Project Objectives

* Store student marks in a 2D NumPy Array
* Analyze overall class performance
* Calculate student-wise averages
* Calculate subject-wise averages
* Find highest and lowest marks
* Identify the class topper
* Practice NumPy's statistical functions

---

## 🛠 Technologies Used

* Python 3
* NumPy

---

## 📂 Dataset

```python
students = np.array([
    [95, 65, 85],
    [89, 72, 88],
    [92, 75, 91]
])
```

### Dataset Structure

| Student   | Subject A | Subject B | Subject C |
| --------- | --------- | --------- | --------- |
| Student A | 95        | 65        | 85        |
| Student B | 89        | 72        | 88        |
| Student C | 92        | 75        | 91        |

---

## 📈 Features

### 1. Display Dataset

Displays all student marks stored in the NumPy array.

---

### 2. Display Shape

```python
students.shape
```

Output:

```text
(3, 3)
```

Meaning:

* 3 Students
* 3 Subjects

---

### 3. Class Statistics

Calculates:

* Total Marks
* Class Average
* Highest Marks
* Lowest Marks

Example:

```python
students.sum()
students.mean()
students.max()
students.min()
```

---

### 4. Student-wise Average

```python
students.mean(axis=1)
```

Output:

```text
[81.67 83.00 86.00]
```

This represents:

| Student   | Average |
| --------- | ------- |
| Student A | 81.67   |
| Student B | 83.00   |
| Student C | 86.00   |

---

### 5. Subject-wise Average

```python
students.mean(axis=0)
```

Output:

```text
[92.00 70.67 88.00]
```

This represents:

| Subject   | Average |
| --------- | ------- |
| Subject A | 92.00   |
| Subject B | 70.67   |
| Subject C | 88.00   |

---

### 6. Topper Detection

```python
topper = np.argmax(student_average)
```

Output:

```text
2
```

Meaning:

```text
Student C is the topper.
```

Topper Percentage:

```text
86.00
```

---

## 📊 Sample Output

```text
==========Student's Performance==========

All Marks:
[[95 65 85]
 [89 72 88]
 [92 75 91]]

Shape: (3, 3)

=========CLASS STATISTICS=========

Total Marks: 752
Class Average: 83.56
Highest Marks: 95
Lowest Marks: 65

==========STUDENT'S PERCENTAGE==========

Student A Percentage: 81.67
Student B Percentage: 83.00
Student C Percentage: 86.00

============SUBJECT-WISE AVERAGE============

Subject A: 92.00
Subject B: 70.67
Subject C: 88.00

=======TOPPER=======

Topper's Student Index: 2
Topper's Percentage: 86.00
```

---

## 📚 Concepts Practiced

* NumPy Arrays
* 2D Arrays (Matrices)
* shape
* sum()
* mean()
* max()
* min()
* axis=0
* axis=1
* argmax()
* Data Analysis Fundamentals

---

## 🎯 Learning Outcomes

Through this project, I learned:

* How to work with 2D NumPy Arrays
* How to analyze tabular data
* How to calculate row-wise and column-wise statistics
* How to identify trends and insights from data
* How NumPy is used in Data Analytics workflows

---

## 🔮 Future Improvements

* Student Grade Calculator
* Pass/Fail Analysis
* Student Ranking System
* User Input Support
* Larger Dataset Analysis
* Data Visualization using Matplotlib
* Integration with Pandas

---
