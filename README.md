# Business Intelligence Performance Dashboard - Amazon Sales Analysis
**Student Name:** Stacy Oboko
**Student ID:** 670722
**Course Code:** DSA3050A — Mid-Semester Examination  

---

## 1. Dataset Profile & Sourcing
* **Data Origin Source:** Publicly Published Enterprise Sales Ledger (Real-world Amazon India E-commerce Transaction Data).
* **Source Verification URL:** (https://www.kaggle.com/datasets/thedevastator/unlock-profits-with-e-commerce-sales-data)
* **Structural Volume:** 128,975 rows | 24 columns

## 2. Business Problem Context
The core objective is transforming fragmented, raw multi-channel operational e-commerce data into structured, strategic intelligence. The raw data contained significant real-world clean-up hurdles: missing transactional values, text formatting variations, mismatched data types, and non-normalized product tracking formats. Building this BI solution streamlines tracking for product mix velocity, fulfillment efficiency, geography-based distribution metrics, and accurate bottom-line performance attributes.

## 3. Comprehensive Power Query Transformation Ledger
The following operational pipeline steps were built inside the Power Query engine to ensure dataset integrity:
* **Structural Cleaning:** Removed multi-layered system duplicate entries and empty structural tracking rows.
* **Schema Definition:** Hard-coded columns to precise datatypes (Dates, Strings, and explicit Text formatting for postal indexing identifiers). Dropped bloated attributes (`Unnamed: 22`, `index`, `fulfilled-by`).
* **Text Formatting:** Cleaned and trimmed whitespace discrepancies across `SKU` and location data. Standardized text case for consistency across the dataset.
* **Column Splitting:** Fragmented alphanumeric structural `SKU` fields by delimiters into modular dimension identifiers (`Product Base Code`, `Pattern Code`, `Size Code`).
* **Advanced M-Logic Integration:**
  * Created custom metrics computing exact order values.
  * Integrated conditional priority columns based on service tiers.
  * Created an isolated custom temporal table (`Dim_Calendar`) via advanced M-script programming to facilitate time-intelligence analytics.
  * Extracted structural segments via text delimiters and structured reference tables to generate aggregate metrics models without disturbing raw base files.

## 4. Built Visual Infrastructure Layout
* **Executive Summary Matrix:** 3 High-level KPI indicators reflecting Net Revenue, Absolute Volumetric Output, and Unique Order Volume counts.
* **Categorical Performance Vectors:** Horizontal distribution bars tracking Revenue across Product lines alongside detailed breakdown ribbon matrix tables.
* **Operational Channels:** Dynamic distribution columns assessing performance differences across fulfillment types.
* **Temporal Trend Line Graphs:** Multi-period chronological charting tracking net daily financial collection vectors.
* **Geographic Spread Projections:** Spatial map tracking financial generation across states.

## 5. Strategic Analytical Executive Summaries
* **Product Mix Strategy:** "Set" and "Kurta" ranges dominate consumer demand curves. Supply networks should realign raw resource assets to backstop production of these core categories.
* **Fulfillment Pipeline Optimization:** Logistics tracking displays optimal fulfillment metrics on Amazon-managed paths vs. merchant-managed setups. Migration of high-turnover SKUs to dedicated warehousing nodes will likely lower churn rates.
* **Geographical Resource Focus:** Marketing allocations should focus on key geographic hotspots (e.g., Maharashtra and Karnataka) to maximize performance outcomes.
