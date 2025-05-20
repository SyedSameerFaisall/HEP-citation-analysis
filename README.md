# HEP Citation Network Analysis (1993–2001)

This repository contains the code and report for a statistical analysis of citation relationships between research papers submitted to **arXiv.org** under the *High Energy Physics – Phenomenology* category (`hep-ph`) between 1993 and 2001.

## 📁 Contents

- `CitationsReport.Rmd` – R Markdown file containing the full analysis and code.
- `CitationsReport.pdf` – The compiled report (knitted from the Rmd).
- `citations.txt` – Citation relationships between papers (FromID → ToID).
- `papers.txt` – Paper submission dates and IDs.

## 📊 Objectives

This project was completed as part of the **UCL Statistical Science Department Take-Home Assessment 2025**, aiming to:

1. **Analyze in- and out-citation distributions**:
   - Compute and visualize citation counts per paper.
   - Perform univariate and bivariate statistical analysis.

2. **Test claims about citation behavior over time**:
   - Fit a linear model to test whether the average number of references (out-citations) per paper increased between 1993 and 2001.

3. **Assess seasonal patterns in paper quality**:
   - Use statistical testing to investigate if papers submitted in autumn/winter receive more citations than those in spring/summer.

## 🛠 Technologies

- **R** (base only – no external libraries)
- **R Markdown** (for reproducible reporting)
- **knitr** (used internally for rendering)

## 📌 Notes

- No third-party packages are used (`library()` is not called).
- The report and code are anonymous and follow the formatting and length constraints defined by UCL.
- Code is fully reproducible and runs assuming the working directory contains the required data files (`citations.txt`, `papers.txt`).

## 🧠 Interpretation Summary

- 📈 Citation behavior varies significantly among papers, with both in- and out-citations being highly skewed.
- ⏳ There is statistical evidence supporting the hypothesis that the number of references per paper increased from 1993 to 2001.
- ❄️ A seasonal effect on paper quality (measured by in-citations) was tested, but the evidence was not conclusive - see report for details.
