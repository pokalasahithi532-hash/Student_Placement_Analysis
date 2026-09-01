# Student Placement Analysis

## Overview

Student Placement Analysis is a machine learning project that predicts student placement outcomes based on academic performance, technical skills, internships, projects, certifications, communication skills, aptitude scores, and backlogs.

The project follows an end-to-end machine learning workflow, from data preprocessing and exploratory data analysis to model training, evaluation, and prediction.

## Dataset

The dataset contains:

- 45,000 training student records
- 5,000 test student records
- 14 predictive features
- Placement Status as the target variable

### Features

- Age
- Gender
- Degree
- Branch
- CGPA
- Internships
- Projects
- Coding Skills
- Communication Skills
- Soft Skills Rating
- Aptitude Test Score
- Certifications
- Backlogs

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Preprocessing

- Loaded and inspected the dataset
- Checked data types and missing values
- Checked duplicate records
- Prepared features and target variable
- Encoded categorical variables

### 2. Exploratory Data Analysis

Analyzed the relationship between placement outcomes and:

- CGPA
- Internships
- Projects
- Coding skills
- Communication skills
- Aptitude scores
- Certifications
- Backlogs

### 3. Feature Engineering

Created additional features including:

- Has_Internship
- Has_Projects
- Has_Backlogs
- Overall_Skill_Score

### 4. Machine Learning Models

Three classification algorithms were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest

The models were compared using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

### 5. Final Model

Random Forest was selected as the final model based on its F1 Score.

The final model was trained and used to generate placement predictions for the test dataset.

## Key Insights

- CGPA showed a positive relationship with placement outcomes.
- Project experience was an important factor in placement prediction.
- Coding skills and certifications were positively associated with placement.
- Internships contributed positively to placement outcomes.
- Backlogs showed a negative relationship with placement.
- Communication and aptitude skills also contributed to placement prediction.

## Output

The project generates:

`placement_predictions.csv`

containing the predicted placement status for the test students.

## Project Structure

```text
Student_Placement_Analysis/
│
├── data/
│   ├── train.csv
│   └── test.csv
│
├── notebook/
│   └── placement_analysis.ipynb
│
├── output/
│   └── placement_predictions.csv
│
├── .gitignore
├── README.md
└── requirements.txt
Conclusion

This project demonstrates an end-to-end machine learning approach for analyzing and predicting student placement outcomes. Multiple classification models were evaluated, with Random Forest selected as the final model based on the evaluation results.


