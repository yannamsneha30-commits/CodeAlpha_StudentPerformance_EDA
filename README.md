# Student Performance Exploratory Data Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on the UCI Student Performance dataset.

The analysis focuses on understanding patterns and relationships between students' demographic, academic, family, and lifestyle characteristics and their final grades.

## Dataset

The dataset used is `student-mat.csv`, which contains student information and academic performance data.

The target variable is:

- `G3` — Final grade

## EDA Questions

The analysis investigates:

1. How are final grades distributed?
2. Is study time associated with final grades?
3. Is the number of previous failures associated with final grades?
4. Is the number of absences associated with final grades?
5. Which numerical variables have the strongest relationship with final grades?
6. Do final grades differ across demographic factors such as gender and school?
7. Is internet access associated with final grades?
8. Is aspiration for higher education associated with final grades?
9. Are family and lifestyle factors associated with final grades?
10. Are there unusual patterns or potential data-quality issues?

## Key Findings

- The average final grade (G3) is approximately 10.42, with grades ranging from 0 to 20.
- G2 has the strongest positive correlation with G3 (0.90), followed by G1 (0.80).
- Previous failures have a negative relationship with final grades.
- Study time shows a small positive relationship with final grade.
- Absences have a very weak linear relationship with G3, with a correlation of approximately 0.03.
- Average final grades differ across demographic groups such as gender and school.
- Students with internet access have a higher average G3 than students without internet access.
- Students who aspire to higher education have a higher average G3 than students who do not report this aspiration.
- Guardian categories show differences in average final grades, while extracurricular activities show only a small difference.
- The dataset contains 38 students with G3 = 0. These observations should be investigated rather than automatically removed.

## Important Note

The findings describe associations in the dataset and should not be interpreted as proof of causation.

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## Project Structure

```text
CodeAlpha_StudentPerformance_EDA/
├── data/
│   └── student-mat.csv
├── notebooks/
│   └── EDA_Project.ipynb
├── visualizations/
│   ├── g3_distribution.png
│   ├── studytime_vs_g3.png
│   ├── failures_vs_g3.png
│   ├── absences_vs_g3.png
│   ├── correlation_heatmap.png
│   ├── sex_vs_g3.png
│   ├── school_vs_g3.png
│   ├── internet_vs_g3.png
│   └── higher_vs_g3.png
└── README.md