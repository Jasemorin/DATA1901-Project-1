# DATA1901-Project-1

Data analysis and presentation using R and Quarto.

## Project Overview

This project investigates the relationship between university students' lifestyle
habits (study hours, sleep, exercise, part-time employment, commute time) and
their academic performance (GPA). The analysis is presented as a reproducible
Quarto report.

## Repository Structure

```
DATA1901-Project-1/
├── report.qmd            # Main Quarto report (edit this file)
├── _quarto.yml           # Quarto project configuration
├── data/
│   └── student_survey.csv  # Survey dataset (100 students, 12 variables)
└── README.md
```

## Requirements

- [R](https://www.r-project.org/) (≥ 4.1)
- [Quarto](https://quarto.org/) (≥ 1.3)
- R packages (install once):

```r
install.packages(c("tidyverse", "knitr", "kableExtra",
                   "ggplot2", "scales", "corrplot"))
```

## Rendering the Report

### HTML output

```bash
quarto render report.qmd --to html
```

### PDF output

```bash
quarto render report.qmd --to pdf
```

The rendered files will appear in the project root directory.

## Dataset

`data/student_survey.csv` contains 100 simulated student survey responses with
the following variables:

| Variable | Description |
|---|---|
| `student_id` | Unique student identifier |
| `age` | Student age (years) |
| `gender` | Gender (Female / Male) |
| `study_hours_per_week` | Weekly study hours outside class |
| `sleep_hours_per_night` | Average nightly sleep (hours) |
| `exercise_days_per_week` | Exercise days per week |
| `part_time_job` | Has a part-time job (Yes / No) |
| `commute_minutes` | One-way commute time (minutes) |
| `gpa` | Grade Point Average (0–7 scale) |
| `faculty` | Faculty of enrolment |
| `year_of_study` | Year of study (1–4) |
| `satisfaction_score` | Life satisfaction score (1–10 scale) |

## Editing the Report

Open `report.qmd` in RStudio or any text editor. The document uses
[Quarto Markdown](https://quarto.org/docs/authoring/markdown-basics.html) with
embedded R code chunks. Update the author names at the top of the file before
submission.
