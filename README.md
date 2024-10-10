# Integrating Copy Number Alterations (CNAs) and Gene Expressions (GEs) - Bioinformatics Research Project

**Summer 2023 - Summer Internship Program**  
**Project Title**: Integrating Copy Number Alterations (CNAs) and Gene Expressions (GEs)  
**Mentor**: Dr. Ibrahim Youssef (ibrahim.youssef@eng1.cu.edu.eg)  
**Project Duration**: Summer 2023

## Project Overview

This project focuses on analyzing multi-platform molecular data from different cancer types—specifically **Lung Squamous Cell Carcinoma (LUSC)** and **Kidney Renal Clear Cell Carcinoma (KIRC)**. The goal is to integrate **Copy Number Alterations (CNAs)** and **Gene Expressions (GEs)** data to identify significant relationships between genomic changes and their impact on gene expression levels.

Through this research, we aim to achieve the following:

1. Identify differentially expressed genes (DEGs) between cancerous and healthy tissues.
2. Conduct multivariable regression analysis to evaluate the effect of CNAs on gene expression levels, using the five most significant DEGs.

## Learning Outcomes

By completing this project, the team will gain:

- **Domain Knowledge** in genetics, including:
  - Gene Expression (GE) analysis
  - Copy Number Alterations (CNAs) analysis
- **Technical Knowledge** in supervised machine learning, specifically:
  - Multivariable regression models
  - Linear, Ridge, and LASSO regression
  - Feature selection techniques

## Requirements

### Data
The data for each cancer type includes:
1. **Gene Expression (GE)**:  
   - Two files for each type (cancerous and healthy tissues)  
     - `type-rsem-fpkm-tcga-t_paired.txt`: GE data for cancerous tissues  
     - `type-rsem-fpkm-tcga_paired.txt`: GE data for healthy tissues  
     - Data is paired, meaning both files have the same number of cases (patients) in the same order.
     
2. **Copy Number Alterations (CNAs)**:  
   - One file per cancer type, representing chromosome segment alterations (arm-level and focal-level).

### Tasks

#### 1. DEGs Identification
For each cancer type:
- Identify **differentially expressed genes (DEGs)** using appropriate hypothesis testing approaches.
- Ensure that the samples are paired for hypothesis testing.

#### 2. Regression Analysis
For each cancer type:
- Perform **multivariable regression** with the GE of one gene as the dependent variable and CNAs as independent variables.
- Focus on the **five most differentially expressed genes** identified in the first task.
- Conduct the analysis on the intersection of cases between GE and CNA datasets.
- Report significant copy number predictors for each gene.

### Deliverables

1. **Code Scripts**:
   - Fully documented Python code with clear comments and at least two functions, saved in separate scripts.
   - Scientific packages used include **NumPy**, **SciPy**, and **Scikit-learn**.

2. **Project Report**:
   - Format the report as a research paper with the following sections:
     - **Introduction**: Overview of the project and its significance.
     - **Methods**: Detailed steps of the analysis, including all software packages used.
     - **Results and Discussion**: In-depth reporting of findings, supported by figures and augmented with textual files or spreadsheets.
     - **Conclusion**: Summary of the overall findings.

## Project Workflow

1. **Data Preprocessing**:
   - Clean and preprocess the GE and CNA datasets.
   - Ensure that paired data is handled correctly for hypothesis testing.
   - Align GE and CNA datasets by intersecting cases.

2. **DEGs Identification**:
   - Apply statistical tests (e.g., paired t-tests) to identify DEGs for each cancer type.
   - Visualize the DEGs through appropriate charts (e.g., heatmaps).

3. **Regression Analysis**:
   - For the five most significant DEGs, build multivariable regression models.
   - Evaluate the influence of CNAs on gene expression.
   - Report significant predictors and visualize the results using figures such as scatter plots or bar graphs.

## Conclusion

This project offers an opportunity to explore the intersection of bioinformatics and machine learning, with a focus on cancer genomics. By integrating CNAs and GEs data, we aim to uncover significant genomic predictors of gene expression changes, providing insights into cancer biology.
