# Student Performance Analytics Using PySpark

## Overview

This beginner project demonstrates a Big Data analytics pipeline using Apache Spark and PySpark. It analyzes student study habits, attendance, and previous exam scores, then uses a machine learning model to predict whether a student passes.

The dataset is synthetic and is intended for learning and demonstration.

## Problem Statement

Analyze student performance data with Apache Spark to explore patterns in exam scores and build a model that predicts pass or fail from study hours, attendance, and previous exam scores.

## Project Objectives

- Load student data from a CSV file using PySpark.
- Clean and prepare the data using Spark DataFrames.
- Summarize results with Spark SQL.
- Train and evaluate a pass/fail classification model using Spark MLlib.
- Visualize exam scores, study hours, and pass/fail counts.

## Dataset

The file `student_performance.csv` contains 500 synthetic student records.

| Column | Description |
|---|---|
| `student_id` | Unique student identifier |
| `study_hours_per_day` | Average hours studied per day |
| `attendance_percentage` | Student attendance percentage |
| `previous_exam_score` | Score on a previous exam |
| `exam_score` | Score on the exam analyzed |
| `passed` | Pass label: `1` if the exam score is at least 50, otherwise `0` |

## Tools and Technologies

- Python
- Apache Spark
- PySpark DataFrames and Spark SQL
- Spark MLlib
- Pandas
- Matplotlib
- Seaborn
- Google Colab or Jupyter Notebook

## Project Workflow

1. Read the CSV file into a Spark DataFrame.
2. Inspect the schema and check for missing values and duplicates.
3. Clean the data and prepare the pass/fail label.
4. Use Spark SQL and DataFrames to summarize student results.
5. Train a logistic regression classifier with Spark MLlib.
6. Evaluate the model and visualize the data.

The classifier uses study hours, attendance, and previous exam score as input features. It does not use `exam_score` as a feature because that score determines the pass/fail label.

## How to Run

1. Download or clone this repository.
2. Open `student_performance_analysis.ipynb` in Google Colab or Jupyter Notebook.
3. Install PySpark by running:

   ```python
   !pip install pyspark
