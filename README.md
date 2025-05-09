
# README: Rare Variant Burden Heritability in ASD

This repository contains all source code, sample data, and analysis files used for the project: **Partitioning Rare Variant Heritability of Autism by Functional Constraint, Sex, and Family Structure**.

## 📁 File Overview

- **`bhr_functional_variant.Rmd`**  
  Main analysis script for estimating burden heritability across functionally grouped rare coding variants. Includes sample data to demonstrate expected data structure and performs the core analysis and figure generation for the report.

- **`heritability_regression.Rmd`**  
  Implements a regression-based heritability estimation approach (liability-scale transformation) used to validate the results from the BHR framework.

- **`sex_female/`, `sex_male/`, `simplex/`, `multiplex/`**  
  Each folder contains scripts mirroring `bhr_functional_variant.Rmd`, used to compute subgroup-specific heritability estimates based on sex and family recurrence.

- **`h2_bygroup.Rmd`**  
  Script for aggregating burden heritability across bins and generating the final plot used in the report.

## 📦 Datasets

This project uses data processed from:
- **SPARK (Simons Foundation Powering Autism Research for Knowledge)**  
  [https://www.sfari.org/resource/spark/](https://www.sfari.org/resource/spark/)

- **UK Biobank Whole Exome Sequencing (WES)**  
  [https://www.ukbiobank.ac.uk/enable-your-research/about-our-data/genetic-data](https://www.ukbiobank.ac.uk/enable-your-research/about-our-data/genetic-data)  

These datasets have restricted access; this code demonstrates the workflow.

## 🧪 Sample Input and Output

- **Sample data** are embedded or loaded via code chunks in `bhr_functional_variant.Rmd` for demonstration purposes.
- Sample outputs include figures and tables that match the report's content.

## ⚙️ System Requirements

- **R version**: ≥ 4.2.0  
- **R packages**:
  - `tidyverse`
  - `data.table`
  - `ggplot2`
  - `gridExtra`
  - `reshape2`
  - `scales`
  - `knitr`
  - `rmarkdown`

Ensure all packages are installed before running the RMarkdown files. You can install missing packages with:

```r
install.packages(c("tidyverse", "data.table", "ggplot2", "gridExtra", "reshape2", "scales", "knitr", "rmarkdown"))
```
## ✍️ Author and Credits

- Code and analysis: Chunni Ji
- Data provided by: Shen Lab (Columbia University) and SPARK Consortium
- Writing assistance: OpenAI ChatGPT (language polishing only)
