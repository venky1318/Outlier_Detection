# Task 28 — Outlier Detection Using Python

## Project Overview

This project demonstrates basic outlier detection using Python, Pandas, NumPy, and Matplotlib.

An employee salary dataset containing 30 sample records is analyzed using a box plot and the Interquartile Range (IQR) method.

The project identifies potential outliers and explains why unusual values should be investigated before making decisions about removing or modifying them.

## Objectives

- Create a box plot for a numerical variable.
- Understand how a box plot represents data distribution.
- Calculate Q1, Q2, Q3, and IQR.
- Calculate lower and upper outlier boundaries.
- Identify potential outlier records.
- Explain the findings from the visualization.
- Preserve the original dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab
- Jupyter Notebook

## Dataset Description

The project uses a manually created employee salary dataset containing 30 fictional employee records.

The dataset includes:

- `employee_id` — Employee identifier.
- `department` — Employee department.
- `monthly_salary_inr` — Monthly salary in Indian Rupees.

One unusually high salary is intentionally included to demonstrate outlier detection.

## Outlier Detection Method

The project uses the Interquartile Range method.

**IQR = Q3 - Q1**

**Lower Boundary = Q1 - 1.5 × IQR**

**Upper Boundary = Q3 + 1.5 × IQR**

A value outside these boundaries is identified as a potential outlier.

## Statistical Results

| Measurement | Result |
|---|---:|
| Total employees | 30 |
| Q1 | ₹48,500 |
| Median | ₹61,000 |
| Q3 | ₹79,500 |
| IQR | ₹31,000 |
| Lower boundary | ₹2,000 |
| Upper boundary | ₹1,26,000 |
| Potential outliers | 1 |

## Identified Potential Outlier

| Employee ID | Department | Monthly Salary |
|---|---|---:|
| EMP030 | Management | ₹3,50,000 |

One unusually high salary exceeds the upper IQR boundary.

The value is retained in the original dataset because an outlier is not necessarily an error.

## Key Observations

1. The middle 50% of salaries lies between ₹48,500 and ₹79,500.
2. One employee salary exceeds the upper boundary of ₹1,26,000.
3. No salaries fall below the lower boundary.
4. The maximum salary is ₹3,50,000.

## Project Files

- `Task_28_Outlier_Detection.ipynb` — Complete Colab notebook.
- `employee_salary_data.csv` — Original employee salary dataset.
- `outlier_results.csv` — Identified potential outliers.
- `outlier_summary.csv` — Statistical and outlier summary.
- `requirements.txt` — Required Python libraries.
- `README.md` — Project documentation.
- `project_report.pdf` — Formal project report.
- `charts/employee_salary_boxplot.png` — Box plot visualization.
- `screenshots/` — Actual execution evidence.

## Conclusion

This project demonstrates how box plots and the IQR method can identify potential outliers in numerical data.

The analysis identifies one unusually high employee salary. The value is preserved for further investigation rather than automatically removed.
