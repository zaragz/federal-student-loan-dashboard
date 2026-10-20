# Federal Student Loan Trends Dashboard (2007–2025)

**Interactive Tableau Dashboard | Excel Data Cleaning | Data Visualization | Trend Analysis**

## Project Overview

This project analyzes trends in the United States federal student loan portfolio from **2007 through Q3 2025**, focusing on outstanding loan balances, recipient counts, and differences among three federal loan programs: Direct Loans, Federal Family Education Loans (FFEL), and Perkins Loans.

Using Microsoft Excel for data preparation and Tableau for interactive visualization, I developed dashboards to examine how the federal student loan portfolio has changed over time and how outstanding balances compare with the number of loan recipients.

**Project Type:** Individual Data Analytics & Visualization Project  
**Tools:** Tableau, Microsoft Excel, CSV  
**University:** University of South Florida  
**Completed:** December 2025 (portfolio revisions: October 2026)

## Project Objectives

- Analyze changes in outstanding federal student loan balances from 2007–2025.
- Compare Direct Loans, FFEL, and Perkins Loans.
- Examine trends in the number of loan recipients.
- Calculate and visualize outstanding balances per recipient.
- Develop interactive dashboards that communicate federal student loan trends.

## Data Source

**Source:** U.S. Department of Education — Federal Student Aid (FSA)

**Dataset:** Federal Student Aid Portfolio Summary

[Official Federal Student Loan Portfolio Data](https://studentaid.gov/data-center/student/portfolio)

The dataset includes outstanding principal and interest balances and recipient counts across federal student loan programs.

**Measurement units:**

- **Dollars:** Outstanding loan balances in billions of USD.
- **Recipients:** Number of recipients in millions.
- **Balance per Recipient:** Thousands of USD per recipient.

## Data Preparation

I used Microsoft Excel to prepare the original portfolio data for visualization.

The preparation process included:

1. Reviewing the original source spreadsheet and identifying relevant loan program fields.
2. Restructuring the data into a consistent tabular format with `Year`, `Dollars`, `Recipients`, and `Loan Program`.
3. Standardizing the Direct Loans, FFEL, and Perkins category labels.
4. Addressing missing year labels in quarterly observations.
5. Selecting one annual observation for each program and year.
6. Exporting the resulting dataset as `Student_Loan_Annual.csv` for Tableau.

The final analysis dataset contains **57 observations: 19 years × 3 loan programs**.

### Annual Observation Method

- **2007–2012:** Original annual records.
- **2013–2024:** Fourth-quarter observations representing federal fiscal year-end.
- **2025:** Third-quarter observations, representing the latest period available in the source file used for this project.

Outstanding balances are point-in-time measures, so quarterly values were not summed to create annual totals.


## Dashboard Previews

### Student Loan Portfolio Analysis

![Student Loan Portfolio Analysis](<img width="1370" height="773" alt="Student_Loan_Portfolio_Analysis" src="https://github.com/user-attachments/assets/06fd005a-5c1b-4150-a8b2-609011e2552a" />)

### Program Comparison & Borrowing Analysis

![Program Comparison and Borrowing Analysis](<img width="1367" height="768" alt="Program_Comparison_Borrowing_Analysis" src="https://github.com/user-attachments/assets/a74d7178-efd6-4d33-889e-547eb376fea4" />)



## Tableau Dashboards

### 1. Student Loan Portfolio Analysis

Examines the evolution of the federal student loan portfolio through:

- Outstanding loan balances by program.
- Student loan recipients by program.
- A dual-axis comparison of Direct Loan balances and recipient counts.
- Outstanding balance per recipient for Direct Loans.

### 2. Program Comparison & Borrowing Analysis

Provides cross-program comparisons using:

- A scatter plot comparing outstanding balances and recipient counts.
- A bar chart comparing outstanding balance per recipient across loan programs.

These visualizations help distinguish changes in total outstanding debt from changes in the number of loan recipients.

## Key Findings

**1. Direct Loans became the dominant federal loan program.**

Outstanding Direct Loan balances increased from approximately **$106.8 billion in 2007 to $1,500.8 billion in Q3 2025**.

**2. FFEL outstanding balances declined.**

FFEL outstanding balances decreased from approximately **$401.9 billion in 2007 to $161.9 billion in Q3 2025**.

**3. Perkins Loans represented a comparatively small portfolio.**

Perkins outstanding balances decreased from approximately **$8.2 billion in 2007 to $2.9 billion in Q3 2025**.

**4. Direct Loan balances increased faster than recipient counts.**

The outstanding Direct Loan balance per recipient rose from approximately **$15,300 in 2007 to $39,500 in Q3 2025**, illustrating growth in the average outstanding portfolio balance per recipient.

These findings describe changes in outstanding balances, not annual loan disbursements or newly issued loans.

## Repository Structure

```text
federal-student-loan-dashboard/
├── README.md
├── data/
│   ├── PortfolioSummary.xlsx
│   └── Student_Loan_Annual.csv
├── tableau/
│   └── Student_Loan_Trends_Dashboard.twbx
└── images/
    ├── Student_Loan_Portfolio_Analysis.png
    └── Program_Comparison_Borrowing_Analysis.png
```

**File descriptions:**

- `PortfolioSummary.xlsx` — Original source, cleaned data, annual preparation steps, and final Tableau-ready worksheet.
- `Student_Loan_Annual.csv` — Final annual analytical dataset.
- `Student_Loan_Trends_Dashboard.twbx` — Packaged Tableau workbook containing both dashboards.
- `images/` — Dashboard screenshots for portfolio preview.

## How to View the Project

1. Download the `.twbx` file from the `tableau/` folder.
2. Open it in a compatible version of Tableau Desktop or Tableau Public.
3. Navigate between the two dashboards to explore the visualizations.
4. Refer to `Student_Loan_Annual.csv` and `PortfolioSummary.xlsx` to examine the underlying data and preparation process.

## Additional Project Links

**Original Project Write-up:**  
[Student Loan Program Trends in the United States — Visual Analytics Journaling](https://visualanalyticsjournaling.blogspot.com/2025/12/student-loan-program-trends-in-united.html)

**Earlier Tableau Public Version:**  
[Student Loan Insights: Borrowing & Program Comparison](https://public.tableau.com/app/profile/zara.gonzalez/viz/Book1_17648241583970/ProgramComparisonBorrowingAnalysis)

*Note: The GitHub workbook contains subsequent data-cleaning and visualization improvements that may not be reflected in the earlier Tableau Public publication.*

## Limitations

- The analysis uses aggregate federal student loan portfolio data rather than individual loan-level records.
- The 2025 observations reflect Q3 rather than a completed federal fiscal year.
- Outstanding balances include principal and interest and should not be interpreted as the amount of new loans issued.
- Balance per recipient is calculated using aggregate program figures and does not represent the distribution of debt across individual recipients.
- Results are descriptive and do not establish the causes of observed changes.

## Author

**Zara Gonzalez**  
University of South Florida  
Information Science — Data Science & Analytics

[GitHub Profile](https://github.com/zaragz)
