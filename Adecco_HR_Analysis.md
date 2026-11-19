# HR Attrition Analysis – Adecco India (Excel)

Adecco India, a mid-sized software company, is losing too many employees, especially junior staff in Sales. In this project I looked at the HR data of 1,470 employees to find out who is leaving, what is linked to it, and where HR should act first.

This is case study DACS12 from the Jobaaj Data Analytics course.

![Dashboard](images/adecco_hr_dashboard.png)

## Dataset

[HR Analytics Case Study on Kaggle](https://www.kaggle.com/datasets/bhanupratapbiswas/hr-analytics-case-study) (the IBM HR attrition data). It has 1,470 employees and 35 columns covering things like department, job level, income, overtime, satisfaction scores, tenure and whether the person left.

## Tools

Excel only: Power Query to load the data, an Excel Table for the clean data, PivotTables with a calculated field, and formulas like COUNTIFS, AVERAGEIF, CORREL, RSQ, T.TEST, INDEX/MATCH and GETPIVOTDATA. Scatter plots with trendlines for the relationship questions.

## Data cleaning

The raw data is kept untouched and all the work is on the Clean sheet, which also has a small block of data quality checks.

- No missing values and no duplicate employees, so nothing had to be filled in or removed
- All scores are within their expected ranges (for example satisfaction is always 1 to 4)
- EmployeeCount, Over18 and StandardHours have the same value for everyone, so I hid them instead of deleting them
- 114 high salaries show up as outliers with the IQR method. They are real salaries of senior staff, so I kept them and only flagged them
- 197 people have NumCompaniesWorked = 0 but more total experience than years at the company. I flagged these rather than changing them
- Added helper columns: a 1/0 attrition flag, text labels for the coded scores, and age, tenure and income groups

## What I found

- Overall attrition is **16.1%** (237 of 1,470), roughly 1 in 6 people
- **Sales** has the highest attrition at 20.6%, and **junior Sales staff (Job Level 1) leave at 42.1%**, about 2.6 times the company average
- People who work **overtime** leave at 30.5%, compared to 10.4% for those who don't
- Single employees (25.5%) and people with **no stock options** (24.4%) leave much more than others
- Leavers earned about **30% less** per month than those who stayed
- The **first 2 years** are the riskiest, with 29.8% attrition
- The three factors most linked to attrition are OverTime, Total Working Years and Job Level, though all the correlations are weak
- The gender difference (17.0% vs 14.8%) is not statistically significant, and job satisfaction and performance ratings hardly change between groups

## Recommendations

1. Start with junior Sales: mentoring and a visible promotion path
2. Cut down on regular overtime, especially in Sales
3. Offer stock options to junior employees as well
4. Review pay at Job Level 1
5. Better onboarding and regular check-ins in the first 2 years

## Workbook

| Sheet | What's in it |
|---|---|
| dashboard | The one-page summary shown above |
| Clean | Cleaned data, helper columns and data quality checks |
| Summary Tables | PivotTables used by the answers |
| Easy | Answers to the 10 basic questions |
| Medium | Answers to the 10 medium questions |
| Chart Data | Small tables that feed the dashboard charts |

The raw data sheet is hidden but still in the file.

## How to open

Download `Adecco_HR_Analysis_Project_Cleaned.xlsx` and open it in Excel 365 or Excel 2021. A few formulas use FILTER, which older versions don't support. The dashboard opens first; the Easy and Medium sheets have each question written above its answer.

## Author

**Manisha Mali**
LinkedIn: [linkedin.com/in/manisha-mali-970b44129](https://www.linkedin.com/in/manisha-mali-970b44129)
