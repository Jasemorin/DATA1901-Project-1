# DATA1901-Project-1

DATA1901 Semester 1 2026 — Group Project 1 Report

## Project Structure

```
DATA1901-Project-1/
├── data/
│   └── 1901_2026_s1_data.xlsx   # Course-provided dataset
├── .gitignore
├── README.md
├── _quarto.yml                   # Quarto project config
├── data1901-banner.html          # Custom report banner
├── report.qmd                    # Main analysis report (edit this)
└── style.css                     # Report stylesheet
```

## Rendering the Report

Install the required R packages, then render:

```r
install.packages(c("tidyverse", "readxl"))
```

```bash
quarto render report.qmd
```

The rendered `report.html` will open in your browser.
