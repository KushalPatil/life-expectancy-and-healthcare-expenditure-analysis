# Healthcare Quality and Expenses Analysis

## Introduction
The purpose of this analysis is to examine the healthcare system of a country and identify the various factors that influence healthcare quality and expenses. The objective is to understand how to reduce health expenses while improving or maintaining the same quality of healthcare. The findings from the analysis will provide insights to policymakers, healthcare officials, and governments for informed decision making.

## Data Collection
Data was collected from the OECD and WHO websites of 39 countries over the 2010-16 period. The sources of data are:
- OECD: https://stats.oecd.org/Index.aspx
- WHO: https://www.who.int/gho/database/en/

The following variables were considered in the analysis:
1. Health Resources:
    a. Hospitals
    b. Hospital Status
    c. Total Equipment
    d. Medical Graduates
    e. Nurse Graduates
2. Health Quality:
    a. Death by respiratory disease
    b. Death by circulatory disease
    c. Death by Cancer
    d. Death by accidents
    a. Mean Schooling years
3. Social Factors:
    a. Mean Schooling years
    b. Population Structure (Age>65)
4. Economic Factors:
    a. Expenditure per capita
5. Medical Procedures:
    a. Diagnostic Exams
6. Insurance:
    a. Public Insurance
    b. Private Insurance

## Data Cleaning
Null values in the data were imputed based on the characteristics of each country and year-over-year changes.

## Exploratory Data Analysis
The following visualizations were created as part of the exploratory data analysis:
- Distribution of Health Expenditure and Life Expectancy
- Correlation Plot
- Health Expenditure vs Life Expectancy

## Model Building
A panel regression model was built to analyze the multi-level data (lower level as time, years). The following models were used in the analysis:
- Pooling Model (baseline model)
- Fixed Effects Model
- Random Effects Model

## Results and Recommendations
The impact of the variables on healthcare quality and expenses was analyzed. The following effects were observed:
- Positive effect on healthcare quality:
  - Number of Hospitals
  - Medical Graduates
  - Nurse Graduates
- Negative effect on healthcare quality:
  - Deaths by any diseases
- Positive effect on healthcare expenses:
  - Public Insurance
  - Hospitals
- Negative effect on healthcare expenses:
  - Private Insurance

Quantitative effects of the variables were visualized.

## Code and Tools Used
The following R packages were used in the analysis:
- Stargazer
- Plm
- Pheatmap

## References
A list of references used in the analysis are provided at the end of the document.

## References 
1) Data Collection, OECD- https://stats.oecd.org/Index.aspx
2) Data Collection, WHO https://www.who.int/gho/database/en/
3) Panel Data Modelling - Panel Data Analysis Fixed & Random Effects - Oscar Torres-Reyna 
4) Panel Data Modelling- Practical Guides To Panel Data Modeling: A Step by Step Analysis 
Using Stata , Hun Myoung Park, Ph.D 
5) Explaining Fixed Effects: Random Effects Modeling of Time-Series Cross-Sectional and 
Panel Data- Andrew Bell, Kelvyn Jones6) Dormont, B., Grignon, M. & Huber, H., 2006. Health expenditure growth: reassessing the 
threat of ageing. Health Economics, 15(9), pp.947-963. 
7) Dreger, C. & Reimers, H.E., 2005. Health care expenditures in OECD countries: a panel 
unit root and cointegration analysis.
8) Steingrímsdóttir, Ó.A., Næss, Ø., Moe, J.O. et al. Trends in life expectancy by education 
in Norway 1961–2009. Eur J Epidemiol 27, 163–171 (2012). 
9) Global, regional, and national life expectancy, all-cause mortality, and cause-specific 
mortality for 249 causes of death, 1980–2015: a systematic analysis for the Global Burden 
of Disease Study 2015 .
10) https://www.who.int/health_financing/documents/report_en_11_deter-he.pd
