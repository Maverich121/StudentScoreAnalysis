# Student Score Analysis

**Application Report — M.Sc. Data Science, TU Dortmund University (Winter Semester 2026/27)**

## Report

[📄 Read the full report (PDF)](report/Data_Science_Report_Dortmund_13.pdf)

## Overview

This project investigates whether Mathematics and Language test scores of 486 students differ significantly by **gender** and **parental education level**. It was completed as part of the application process for the M.Sc. Data Science programme at TU Dortmund University, Department of Statistics.

## Research Questions

1. Is there a statistically significant difference between male and female students in their Mathematics and Language scores?
2. Is there a difference in scores across parental education levels? If so, which groups differ from each other?

## Key Findings

- **Gender:** Male students scored significantly higher in Mathematics (*t* = 3.776, *p* < 0.001), while female students scored significantly higher in Language (*t* = −6.409, *p* < 0.001).
- **Parental Education:** Scores differ significantly across education levels in both subjects (Math: *F* = 6.223, *p* < 0.001; Language: *F* = 14.241, *p* < 0.001). Students whose parents hold only a high school diploma scored significantly lower than all other groups.

## Methods

- Descriptive statistics (mean, median, standard deviation, boxplots, histograms)
- Two-sample *t*-test for gender comparisons
- One-way ANOVA and Kruskal–Wallis test for parental education comparisons
- Post-hoc: Tukey's HSD and Dunn's test with Bonferroni correction
- Assumption checks: Shapiro–Wilk (normality), Levene's test (homogeneity of variances)

## Repository Structure

```
StudentScoreAnalysis/
├── README.md
├── data/
│   └── Scores.csv              # Raw dataset (486 students, 972 rows)
├── report/
│   └── Data_Science_Report_Dortmund_13.pdf   # Full 10-page report
└── src/                        # Analysis code (coming soon)
```

## Data

The dataset (`data/Scores.csv`) contains 972 observations for 486 students, each assessed in both Mathematics and Language (scores 0–100). Variables include:

| Variable | Description |
|---|---|
| `student_id` | Unique student identifier |
| `gender` | `male` or `female` |
| `parental.level.of.education` | `high school`, `associate's degree`, `bachelor's degree`, `master's degree` |
| `subject` | `math` or `language` |
| `score` | Test score (0–100) |

## Tools

- Python (NumPy, pandas, SciPy, Matplotlib, scikit-posthocs)

## Author

Mert Görgülü

## License

This project is for academic purposes.
