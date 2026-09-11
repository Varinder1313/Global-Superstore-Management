# README / Methodology
## Data Analyst Assessment — Global Superstore Profitability Analysis

---

## 1. Overview

This project analyzes the **Global Superstore** dataset to identify where profit is being lost
despite healthy sales, and to give management clear, actionable recommendations. It was
completed as part of the VirtuBox Data Analyst assessment.

---

## 2. Business Problem

Management wants to move from a "grow sales" mindset to a "grow **profitable** sales" mindset.
This analysis investigates where discounting, product category mix, and regional cost
structures are eroding profit margin, and what management can do about it.

---

## 3. Dataset

| Detail | Value |
|---|---|
| Name | Global Superstore |
| Records | 51,290 orders |
| Fields | 31 columns |
| Coverage | 2011–2014, 7 markets (US, EU, APAC, LATAM, EMEA, Africa, Canada) |

**Source:** Publicly available Global Superstore dataset (Kaggle / Tableau sample data).

---

## 4. Methodology

### Step 1 — Data Collection
Identified and imported the Global Superstore dataset into the working environment
(**Worksheet: Data**).

### Step 2 — Problem Definition
Defined the business problem, 3–5 guiding analysis questions, and 2+ testable hypotheses
(**Worksheet: Q2**).

### Step 3 — Data Cleaning & Processing
Processed the raw dataset into an analysis-ready format (**Worksheet: Processed Data**),
including:
- Handling missing values (e.g., missing postal codes, flagged rather than dropped)
- Removing duplicate order lines
- Correcting and standardizing data types (dates, currency fields)
- Creating calculated fields: **Profit Margin %**, **Delivery Days**, **Margin Category**,
  **Profit Outlier Flag**
- Categorizing and aggregating data by Category, Sub-Category, Market, Region, and Segment
- Identifying outlier/unusual profit records

Major cleaning decisions and their justification are documented in **Worksheet: Q3**.

### Step 4 — Exploratory & Descriptive Analysis
Performed aggregation and comparison across Category, Sub-Category, Market, Segment, and
Discount level to surface business insights (**Worksheet: Q4**), and investigated one
unexpected finding in depth (**Worksheet: Q5**).

### Step 5 — Data Quality & Limitations Review
Identified data-quality issues, analytical risks, and the boundaries of what the dataset can
and cannot support (**Worksheet: Q6**).

### Step 6 — Recommendations
Translated insights into 3 prioritized, actionable recommendations for management, each tied
to a measurable outcome (**Worksheet: Q7**).

### Step 7 — Dashboard
Built an interactive Google Looker Studio dashboard summarizing KPIs, trends, and segment
performance for a business (non-analyst) audience (**Worksheet: Q8**).

### Step 8 — Presentation
Built a 7-slide management presentation summarizing the business problem, methodology, key
findings, deep-dive insight, recommendations, expected impact, and limitations.

---

## 5. Tools Used

| Purpose | Tool |
|---|---|
| Data processing & analysis | Python (Pandas, NumPy) |
| Dashboard | Google Looker Studio |
| Presentation | PowerPoint (.pptx) |
| Data storage | Google Sheets |

---

## 6. Key Findings (Summary)

- Overall profit margin across the business: **11.6%** on $12.6M in sales
- **Furniture** is the weakest category at **6.9% margin**, versus ~14% for Technology and
  Office Supplies
- **Tables** is the single largest loss-making sub-category: **-8.5% margin, -$64K profit**
- A clear relationship exists between discount level and profitability: average margin turns
  negative once discounts exceed roughly **20%**
- **EMEA** is the weakest-performing market on margin (**5.4%**) despite meaningful sales volume

---

## 7. Limitations

- Profit figures reflect the dataset's provided field, not an audited P&L — dollar impact
  should be validated against finance records before action
- Discount reason (negotiated deal, promotion, clearance) is not captured, so the
  discount–margin relationship is a strong correlation, not proven causation
- The dataset does not support concluding that all discounting should stop — some discounts
  may protect volume or key accounts in ways this data can't show

---

## 8. AI Usage

AI (Claude) was used in a limited, supporting capacity — checking code for small errors,
polishing chart formatting, and improving the clarity of written explanations. All dataset
selection, cleaning decisions, hypotheses, calculations, insights, and recommendations were
independently performed and verified. Full detail is documented in **Worksheet: Q10**.

---

## 9. Folder Contents

1. **Google Sheet** — all worksheets (Data, Q1–Q7, Q10)
2. **Code** — Python notebook/script
3. **Presentation** — 5–7 slide management deck (.pptx)
4. **README / Methodology** — this document
