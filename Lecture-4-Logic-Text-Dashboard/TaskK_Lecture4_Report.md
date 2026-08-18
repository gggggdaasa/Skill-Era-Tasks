# TaskK – Lecture 4 Implementation Report

**Student:** Mustafa Mahmoud Ali  
**Phone:** 01032340302  
**Email:** shroh1520132020sh@gmail.com

## Objective
The workbook applies IF, AND, OR, and text functions to the 24 records supplied for Lecture 4 and presents the outcomes in a dashboard.

## Data preparation
The original ID, Gender, and Age fields were preserved. Formula-driven derived columns were added so the file can be audited and recalculated in Excel.

## New columns and rationale
| Column | Formula concept | Purpose |
|---|---|---|
| Answers (Q1) | IF + AND | Returns Yes only when Gender is M and Age is greater than 34. |
| Answers (Q2) | IF + OR | Returns Yes when Gender is F or Age is less than 25. |
| Gender Label | IF | Converts M/F codes into Male/Female labels. |
| Age Group | Nested IF | Segments ages into Under 25, 25-34, and 35+. |
| Record Code | CONCAT + TEXT + UPPER | Creates a standardized identifier such as ID-001-M. |
| Logic Summary | CONCAT | Combines descriptive fields and both logic outcomes for review. |

## Dashboard
The Dashboard sheet contains KPI cards for total records, Q1 Yes, Q2 Yes, and average age. It also contains summary tables and charts for logic outcomes, gender distribution, and age groups.

## Quality checks
Q1 uses a strict `>34` condition, while Q2 uses a strict `<25` condition. Formulas are retained instead of static answers. After recalculation, the workbook shows **24 total records**, **4 Q1 Yes results**, **14 Q2 Yes results**, and an **average age of 30.625**.
