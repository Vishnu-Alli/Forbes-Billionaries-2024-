# Forbes-Billionaries-2024-
A comprehensive Power BI dashboard analyzing the Forbes Billionaires 2024 dataset. This project provides insights into global wealth distribution, billionaire demographics, industry trends, and geographical statistics using interactive data visualizations and DAX measures.



## 🔍 Overview

The dashboard provides:
- **Top 10 Billionaires by Net Worth**
- **Wealth Distribution by Country & Industry**
- **Gender and Age Distribution**
- **Year-on-Year Net Worth Changes**
- **Top 10 Companies/Enterprises**
- **Interactive Map of Billionaires by Country**

## 📊 Tools & Technologies

- **Power BI**
- **Microsoft Excel** (for initial data formatting)
- **DAX** (Data Analysis Expressions)

## 🧠 Key Insights

- United States leads with the highest number of billionaires.
- Technology and Finance dominate among billionaire industries.
- There is a significant gender disparity in billionaire representation.
- Net worth is highly skewed — top 1% hold disproportionate wealth.

## 🧮 Sample DAX Measures

DAX
Total Billionaires = DISTINCTCOUNT('Billionaires'[Name])
Average Net Worth = AVERAGE('Billionaires'[Net Worth])
Top Country = CALCULATE(MAX('Billionaires'[Country]), TOPN(1, VALUES('Billionaires'[Country]), [Net Worth], DESC))
