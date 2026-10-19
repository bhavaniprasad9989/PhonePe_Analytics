
# 📊 PhonePe Transaction Analysis Dashboard | Power BI

**An Interactive Data Analytics Project Using Power BI, DAX & Power Query**

---

## 📌 Project Overview

The **PhonePe Transaction Analysis Dashboard** is an interactive business intelligence project developed using Microsoft Power BI. It helps explore digital payment transaction activity, transaction values, user behavior, service categories, payment statuses, and weekday-versus-weekend patterns.

The dashboard presents key performance indicators (KPIs), time-based trends, user comparisons, and interactive visualizations to make transaction data easier to understand.

This project demonstrates practical skills in data analysis, DAX measures, dashboard development, data visualization, and business intelligence.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze total transaction volume and transaction value.
- Monitor month-over-month changes in transaction performance.
- Identify the top 5 users by transaction value.
- Compare transaction values across services and service types.
- Understand user distribution across age segments.
- Compare transaction activity on weekdays and weekends.
- Examine transaction values across payment statuses.
- Build an interactive dashboard using slicers and report-page tooltips.
- Present data in a clear and business-friendly format.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Power BI | Dashboard development and reporting |
| DAX | KPI calculations and analytical measures |
| Power Query | Data preparation and transformation |
| Data Modeling | Organizing tables and analytical fields |
| Data Visualization | Presenting trends, comparisons, and patterns |
| GitHub | Project documentation and portfolio management |

---

## 📊 Dashboard Features

### 1. KPI Cards

The dashboard includes KPI cards for monitoring important transaction metrics:

- **Total Users** — user count according to the configured measure.
- **Total Transactions** — transaction volume according to the configured measure.
- **Total Transactions Value** — aggregate transaction value.
- **Transactions Per Day** — daily transaction activity according to the configured calculation.
- **Transaction Value MoM %** — month-over-month change in transaction value.
- **Transaction MoM %** — month-over-month change in transaction volume, subject to verification of the measure definition.

### 2. Transaction Value Analysis

Analyze transaction values across services and service categories to explore their contribution to overall transaction activity.

### 3. Monthly Trend Analysis

Explore monthly transaction values and month-over-month changes to understand how transaction performance varies over time.

### 4. Top 5 User Analysis

Identify the five users with the highest transaction values and compare their transaction activity.

### 5. Age Segment Analysis

Explore the distribution of users across age segments using a donut chart.

### 6. Weekday vs. Weekend Analysis

Compare transaction activity on weekdays and weekends to identify differences in usage patterns.

### 7. Payment Status Analysis

Explore transaction values across payment statuses to understand how transaction activity is distributed among the available statuses.

### 8. Interactive Tooltips

The report includes tooltip pages that provide additional breakdowns through visualizations such as:

- Service-type pie charts
- Weekday-versus-weekend comparisons
- Monthly trend charts
- Service-type bar charts
- Payment-status column charts

### 9. Interactive Filters

The dashboard includes slicers for:

- Month
- Payment Status

These filters allow users to explore the report under different selections. Visual interactions depend on the configured Power BI settings.

---

## 📈 Business Questions

This dashboard helps investigate the following questions:

1. What is the total transaction volume?
2. What is the overall transaction value?
3. How does transaction value change month over month?
4. Which services contribute the most to transaction value?
5. Which five users have the highest transaction values?
6. How are users distributed across age segments?
7. How does transaction activity differ between weekdays and weekends?
8. How is transaction value distributed across payment statuses?
9. How does transaction activity change when different months are selected?
10. What additional patterns can be explored using interactive tooltips?

The answers should be determined from the actual dataset, active filters, and validated measure definitions rather than assumed in advance.

---

## 🧮 DAX & Analytical Measures

DAX (Data Analysis Expressions) is used in Power BI to create calculations and analytical measures.

### Example: Transaction Value Month-over-Month %

```dax
Transaction Value MOM% =
DIVIDE(
    [Total Transactions Value] - [Transaction Value PM],
    [Transaction Value PM],
    0
)
```

**Purpose:** Calculates the percentage change in transaction value compared with the previous month's transaction value.

**Formula:**

Month-over-Month % =

(Current Month Value − Previous Month Value)
÷ Previous Month Value

The result is normally formatted as a percentage in Power BI.

**Note:** The measure `[Transaction Value PM]` must correctly calculate the previous month's value. Validate its date context and the handling of missing or zero previous-month values before relying on the result.

---

## 🗂️ Data Model

The report metadata identifies the following tables:

- `All_Transactions` — transaction-related fields.
- `All_Users` — user-related fields.
- `Date_Table` — calendar and date-related fields.
- `Measure` — a table used to organize measures.

The exact table relationships, source transformations, column definitions, and data grain should be verified in Power BI Desktop.

---

## 📂 Project Files

The repository contains the Power BI report and its supporting documentation.

- **Power BI Report:** `Phone_Pay_Analysis_2.pbix`
- **README:** Project documentation
- **Dashboard Screenshot:** 
`![PhonePe Dashboard](PhonePe Payments Insights Dashboard.png.png)`
---

## 🚀 How to Open the Dashboard

Follow these steps to explore the project:

1. Open this GitHub repository.
2. Locate `Phone_Pay_Analysis_2.pbix`.
3. Click the file and download it to your computer.
4. Install Microsoft Power BI Desktop if it is not already installed.
5. Open the downloaded `.pbix` file in Power BI Desktop.
6. Wait for the report to load.
7. Use the Month and Payment Status slicers to explore different selections.
8. Select chart categories to examine supported cross-filtering behavior.
9. Hover over relevant visuals to explore the configured tooltip pages.
10. Review the DAX measures and data model in Power BI Desktop.

---

## 💡 Key Learnings

Through this project, I developed practical experience in:

- Creating an interactive Power BI dashboard.
- Developing and organizing DAX measures.
- Designing KPI cards and analytical visualizations.
- Exploring transaction and user-related data.
- Comparing performance across categories and time periods.
- Configuring interactive slicers and report-page tooltips.
- Organizing analytical tables and date-related fields.
- Documenting business questions and analytical assumptions.
- Preparing a data analytics project for a professional portfolio.

---

## ⚠️ Limitations

- The analysis depends on the completeness and quality of the supplied dataset.
- Dashboard values may change according to active slicers and visual interactions.
- KPI accuracy depends on the definitions and implementation of the underlying DAX measures.
- Month-over-month calculations depend on a correctly configured date table and previous-month logic.
- Transaction success rates should not be inferred from payment statuses without validating the status definitions and calculation logic.
- User-level comparisons depend on the available user identifiers and transaction records.
- The project does not establish that the dataset represents all actual PhonePe transactions.
- Findings should not be treated as official PhonePe business results unless the data source and authorization establish that status.

---

## 🔮 Future Improvements

Potential enhancements include:

- Add a verified transaction success-rate KPI.
- Include additional date-based comparisons and year-over-year analysis.
- Improve drill-through navigation between report pages.
- Add validated business insights supported by actual dashboard results.
- Optimize DAX measures and model performance.
- Publish a Power BI Service version if the data-sharing permissions allow it.
- Add a dashboard screenshot and a short project walkthrough to the GitHub repository.

These are potential future enhancements, not claims that all features are currently implemented.

---

## 📝 Conclusion

The PhonePe Transaction Analysis Dashboard demonstrates how Power BI can be used to organize transaction data into an interactive analytical report.

By combining KPI cards, monthly trends, user comparisons, service-level analysis, payment-status breakdowns, and interactive tooltips, the project provides a structured way to explore transaction behavior.

The project strengthened my practical understanding of Power BI, DAX, data visualization, and business intelligence while providing a foundation for further analytical improvements.

---

## 👨‍💻 Skills Demonstrated

`Microsoft Power BI` · `DAX` · `Power Query` · `Data Analysis` · `KPI Development` · `Data Visualization` · `Business Intelligence` · `Dashboard Design`

---

**Project:** PhonePe Transaction Analysis Dashboard  
**Platform:** Microsoft Power BI  
**Project Type:** Data Analytics & Business Intelligence  
**Purpose:** Professional Analytics Portfolio

