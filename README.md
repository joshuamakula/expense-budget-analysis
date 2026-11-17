Expense Budget Analysis

Analysis of departmental expenses against planned budgets. The project cleans a messy customer dataset, flags over-budget and on-budget spending, summarizes results in a pivot table, and presents them in a dashboard.
<img width="904" height="466" alt="clean data" src="https://github.com/user-attachments/assets/766354b0-f92f-473b-86da-8a463e15ffe7" />


## Contents
- `raw/` - original customer file as received
- `clean/` - cleaned expense dataset
- `excel/` - final workbook (Budget Status, pivot table, chart, conditional formatting, dashboard)
- `docs/` - screenshots and method notes

## Data
Columns: Department, Category, Month, Planned Budget ($), Actual Spend ($), Notes.

## Cleaning steps
1. Converted text numbers in Planned Budget and Actual Spend to numeric values.
2. Removed blanks and duplicate rows.
3. Standardized department, category, and month names.

## Analysis
- **Budget Status:** On Budget when Actual Spend is less than or equal to Planned Budget; Over Budget when Actual Spend is greater.
- **Overspend flag:** Rows where overspend exceeds 20% of Planned Budget are highlighted with conditional formatting.
- **Pivot table:** Total planned vs actual spend by department.
- **Chart and dashboard:** Visualize the difference between planned and actual spend per department.

## How to open
Open `clean.xlsx` in Microsoft Excel. Start from the Dashboard sheet.

## Key findings
- Total planned budget: $2,756,656. Total actual spend: $3,181,620.
- Total overspend: $424,964 (15.4%). All 7 departments spent more than planned.
- 2 departments exceeded the 20% overspend threshold: Operations (26.9%) and Logistics (24.2%).
Method: data cleaned, Budget Status assigned, overspend flagged, totals summarized by department.

<img width="1118" height="184" alt="image" src="https://github.com/user-attachments/assets/9f5357b6-6a3c-4adc-80ab-a069392dfb15" />

## Findings and recommendations
1. Review Operations and Logistics first. They exceed the 20% overspend threshold.
2. Investigate why Marketing, HR, and IT each overspent by more than 12%.
3. Set monthly checkpoints so overspend is caught before the year closes, not after.
4. Confirm the source of Actual Spend values and whether any were timing or one-off costs.
5. Keep the cleaning rules documented so future data loads are handled the same way.

<img width="748" height="408" alt="Dashboard" src="https://github.com/user-attachments/assets/6cf8426b-db16-4b6c-b67e-d15ef8603647" />



## License
[EBA v1.0]
