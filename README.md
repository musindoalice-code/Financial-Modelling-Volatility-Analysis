# Exploratory Financial Data Modelling & Volatility Analysis

## 📌 Project Overview
Developed programmatic data workflows utilizing Python to process unstructured transactional general ledgers, handle missing rows, clean currency variables, and deploy mathematical similarity algorithms to uncover leakage vectors.

## 🛠️ Tech Stack & Packages
- **Language:** Python 3.x (Databricks-compatible)
- **Data Engineering:** Pandas, NumPy
- **String Distance Algorithms:** RapidFuzz (Levenshtein Distance Metric & Token Sort Sorting Ratios)

## 📊 Continuous Controls Validation
- Employs **Fuzzy Logic matching** across text parameters to capture hidden variations that exact SQL queries bypass.
- Evaluates multi-dimensional conditions simultaneously (text similarity index + timeline windows + custom numeric variances).

# Fuzzy Audit Findings Report

## 1. Overview

The objective of this audit was to identify potential duplicate invoices and unusual payments using Python and fuzzy matching techniques in Databricks. The analysis compared vendor names, invoice dates and invoice amounts to identify transactions requiring further investigation.

## 2. Data Quality and Cleaning

The ledger initially contained **[insert initial row count]** invoice records. After standardising dates and amounts and removing records with missing or invalid required fields, **[insert retained row count]** records remained for analysis.

## 3. Duplicate Invoice Findings

The exact duplicate check identified **[insert count] rows with repeated invoice IDs**. The fuzzy matching process flagged **[insert count] potential duplicate invoice pairs** based on vendor similarity, a maximum 30-day date difference and an amount variance of no more than 2%.

These results are potential exceptions and do not confirm fraudulent activity.

## 4. Vendor Risk Analysis

The vendors appearing most frequently in flagged pairs were **[insert vendor names]**. These vendors should be reviewed to determine whether the matches result from duplicate processing, inconsistent vendor naming or legitimate transactions.

## 5. Unusual Payments

The statistical outlier analysis identified **[insert count] unusual invoice amounts** using the interquartile range method. These transactions require contextual review because an unusual amount does not necessarily indicate fraud.

## 6. Recommended Audit Actions

For each flagged case, the auditor should inspect:
- Original invoices and invoice numbers.
- Vendor master records and any approved aliases.
- Purchase orders, contracts and goods-received records.
- Invoice dates, amounts, VAT and payment records.
- Approval workflows and supporting documentation.
- Whether the same invoice was paid more than once.

Cases should be cleared when sufficient evidence supports a legitimate transaction. Cases with unresolved discrepancies should be escalated under the organisation's audit procedures.

## 7. Conclusion

The fuzzy audit provides a structured way to prioritise potential duplicate invoices and unusual payments. The findings should be validated against source documents and payment records before any conclusion about fraud or financial loss is reached.
