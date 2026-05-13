# Student Score Analysis

**Application Report — M.Sc. Data Science, TU Dortmund University (Winter Semester 2026/27)**

## Report

[📄 Read the full report (PDF)](report/Data_Science_Report_Dortmund_13.pdf)

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

## License

This project is for academic purposes.
