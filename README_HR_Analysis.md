# Adecco India — HR Attrition Analysis

An Excel-based HR analytics project analyzing employee attrition at "Adecco India," using the well-known IBM HR Employee Attrition dataset (1,470 employees, 35 attributes). The workbook moves from raw data to a set of guided business questions to a summary dashboard with KPIs and charts.

## Contents

The workbook (`Adecco_HR_Analysis_Project.xlsx`) has 7 sheets:

| Sheet | Description |
|---|---|
| `Dashboard` | Summary dashboard with headline KPIs — overall attrition rate, total employees, employees who left, average tenure, % working overtime, and average income of employees who left — backed by pivot charts. |
| `Analysis` | Working copy of the employee dataset (1,470 rows × 35 columns) with an added `Attiration_Yes` helper column for correlation analysis. |
| `Summary Tables` | Pivot table summaries built from the dataset (attrition by department, job role, etc.). |
| `Easy` | 10 beginner-level business questions with worked answers (e.g. overall attrition rate, attrition by department, average age/income of employees who left, overtime patterns). |
| `Medium` | 10 intermediate-level questions with worked answers, including a correlation analysis of the top factors driving attrition. |
| `WA_Fn-UseC_-HR-Employee-Attriti` *(hidden)* | The original, untouched source dataset. |
| `Sheet2` *(hidden)* | Pivot table helper/cache sheet. |

The workbook includes 17 pivot tables and 13 charts in total, feeding the dashboard and the summary tables.

### Dataset

The source data is the classic IBM/Kaggle **HR Employee Attrition** dataset — 1,470 employee records with 35 fields covering demographics (age, gender, marital status), job details (department, job role, job level, business travel), compensation (daily/hourly/monthly rate, monthly income, stock option level), satisfaction scores (job, environment, relationship, work-life balance), and tenure (years at company, years in current role, years since last promotion, years with current manager).

### Business questions answered

**Easy**
1. What is the overall attrition rate at Adecco India?
2. Which department has the highest attrition rate?
3. What is the average age of employees who have left the company?
4. How does job satisfaction vary across different job roles?
5. Is there a significant difference in attrition rates between male and female employees?
6. What is the average monthly income of employees who have left the company?
7. How does distance from home impact employee attrition?
8. What is the distribution of performance ratings among employees?
9. How many employees work overtime regularly?
10. What is the average number of years employees have worked at Adecco India?

**Medium**
1. What are the top three factors contributing to employee attrition at Adecco India?
2. How does the attrition rate vary with different levels of job involvement?
3. Is there a relationship between employee age and job satisfaction?
4. How does marital status impact employee attrition?
5. What is the impact of training on employee attrition?
6. How does work-life balance affect employee performance ratings?
7. What is the effect of stock options on employee attrition?
8. How does employee tenure relate to job satisfaction?
9. What is the impact of business travel on job satisfaction?
10. How do years since last promotion affect employee performance?

## Getting started

1. Download `Adecco_HR_Analysis_Project.xlsx`.
2. Open it in Microsoft Excel (2016+ recommended) or another spreadsheet app that supports pivot tables and charts, such as LibreOffice Calc.
3. Start on the `Dashboard` sheet for the headline KPIs, then explore `Easy` and `Medium` for the question-by-question breakdowns, and `Analysis` / `Summary Tables` for the underlying data and pivots.

## Requirements

- Microsoft Excel 2016 or later (recommended, for full pivot table and chart fidelity)

## Author

Manisha Mali
