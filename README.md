# Vendor Payment Performance & Payee Health Scorecard

## <img width="1376" height="753" alt="image" src="https://github.com/user-attachments/assets/738cb5a7-3a07-4866-8d5f-9932ca77fd95" />

## Project Overview

This project analyzes vendor-level payment performance and outstanding invoice balances using Microsoft Excel. It demonstrates how finance operations teams can monitor payment failures, evaluate vendor health, analyze invoice aging, and prioritize vendors for proactive follow-up.

The project uses a synthetic portfolio dataset and a custom vendor health scoring model to classify vendors into Healthy, Monitor, and High Risk categories.

**Disclaimer:** This is an independent portfolio simulation using synthetic data. It is not based on Amazon's internal systems, Oracle records, or actual vendor transactions.

## Business Problem

Recurring payment failures, overdue invoices, and accumulating outstanding balances can create operational challenges for finance teams and vendors.

The objective of this project is to build a vendor-level monitoring dashboard that helps identify payment issues, compare vendor performance, and prioritize accounts requiring further review.

## Tools & Technologies

- Microsoft Excel
- Excel formulas: `IF`, `COUNTIF`, `COUNTIFS`, `SUMIF`, `SUMIFS`, `VLOOKUP`, `IFERROR`, `MAX`, and `MIN`
- Excel Tables and data organization
- PivotTables and charts
- Conditional formatting
- KPI reporting and dashboard visualization
- Vendor risk scoring and performance analysis

## Key Business Questions

- Which vendors have the highest outstanding balances?
- Which vendors experience recurring payment failures?
- How much outstanding value falls into each invoice aging bucket?
- Which vendors have the highest payment failure rates?
- Which vendors should be prioritized for proactive review?
- How can vendor-level indicators be summarized in a health scorecard?

## Dashboard Overview

The interactive Excel dashboard includes four KPI cards and six analytical sections.

### KPI Cards

| KPI | Current Result |
|---|---:|
| Total Vendors | 20 |
| High-Risk Vendors | 15 |
| Vendors to Monitor | 5 |
| Failed Payment Attempts | 40 |

These results reflect the current workbook and its custom scoring rules.

### Analytical Sections

**1. Vendor Health Distribution**

Summarizes the number of vendors classified as High Risk, Monitor, or Healthy.

**2. Outstanding Balance by Vendor**

Compares outstanding invoice balances across vendors to identify accounts requiring attention.

**3. Invoice Aging Analysis**

Groups outstanding amounts into the following buckets:

- 0–30 Days
- 31–60 Days
- 61–90 Days
- More than 90 Days
- Not Yet Overdue

The reporting date used in the workbook is 14 October 2026.

**4. Payment Attempt Status**

Summarizes 420 payment attempts:

| Payment Status | Attempts |
|---|---:|
| Successful | 335 |
| Failed | 40 |
| Pending | 45 |
| **Total** | **420** |

**5. Vendor Payment Failure Rate**

Compares vendor payment failure rates to help identify vendors with recurring payment issues.

**6. Vendor Health Scorecard**

Displays vendor-level outstanding balances, failed payments, overdue invoice counts, health scores, and risk classifications.

## Vendor Health Scoring Methodology

A custom scoring model combines three indicators:

- Payment failure rate
- Overdue invoice count
- Outstanding balance relative to the largest vendor balance

The score ranges from 0 to 100, with lower scores indicating greater potential risk.

The current classification thresholds are:

| Health Score | Risk Category |
|---|---|
| 70 and above | Healthy |
| 50 to below 70 | Monitor |
| Below 50 | High Risk |

These thresholds are project-specific assumptions rather than an industry-standard model.

## Business Value

The dashboard demonstrates how Excel-based analytics can support finance operations by:

- Highlighting vendors with substantial outstanding balances.
- Identifying recurring payment failures and follow-up priorities.
- Monitoring overdue amounts across aging buckets.
- Comparing vendor payment performance.
- Standardizing vendor-level reporting.
- Presenting operational indicators in a consolidated scorecard.

## Data Quality & Limitations

- All data is synthetic and intended for educational and portfolio use.
- Duplicate invoice submissions may inflate preliminary outstanding balances.
- Outstanding amounts should be reconciled before being treated as final payable liabilities.
- Payment failure rates depend on the payment attempts recorded in the workbook.
- The vendor health score is a custom analytical indicator, not an official Amazon or industry scoring standard.
- Vendors classified as High Risk should be reviewed against their underlying metrics rather than judged by the score alone.

## Project Files

- `Vendor_Payment_Performance_Payee_Health_Scorecard.xlsx` — Excel workbook containing vendor analysis and dashboard.
- `README.md` — Project documentation.

## Skills Demonstrated

Excel Analytics | Finance Operations | Vendor Payment Analysis | Invoice Aging | Outstanding Balance Monitoring | Payment Failure Analysis | Risk Classification | KPI Reporting | Dashboard Development

## Disclaimer

This project was developed independently for educational and portfolio purposes. All data is synthetic and does not represent actual company, customer, or vendor records.
