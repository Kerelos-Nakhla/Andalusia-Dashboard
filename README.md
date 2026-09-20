# Andalusia Healthcare Performance & Financial Intelligence Dashboard

<p align="center">
  <b>Executive Healthcare Analytics, Outpatient Volume & Revenue Target Tracking in Power BI</b>
</p>

---

## Executive Overview
The **Andalusia Healthcare Analytics Dashboard** is an enterprise hospital management and clinical revenue intelligence system built in Power BI for Andalusia Hospitals Group. The dashboard monitors clinical throughput, patient consultation volumes (C/V), baseline expectations, and actual revenue realization across specialized medical departments and geographic business units.

### Core Metrics (Calculated Directly from Actual Dataset)
- **Actual Realized Revenue:** **$575,194,957.95** (~$575.2M)
- **Target Revenue Budget:** **$724,887,777.62** (~$724.9M)
- **Baseline Revenue Benchmark:** **$706,296,549.89** (~$706.3M)
- **Historical Comparative Revenue:** **$463,678,886.83** (~$463.7M)
- **YoY Revenue Growth:** **+24.05%** over historical period
- **Budget Target Achievement:** **79.35%** of target revenue achieved
- **Departmental Partitions:** 146 clinical billing partitions analyzed across Cardiology, Orthopedics, Pediatrics, Oncology, Internal Medicine, and Surgical departments

---

## Business Problem & Objectives
1. **Revenue Target Gap Analysis:** Identify clinical departments lagging behind their allocated budgetary targets and isolate whether volume (consultations) or cost per visit (C/V) is the primary driver.
2. **Business Unit Performance:** Compare performance across hospital branches and countries to optimize resource allocation and clinical staffing.
3. **Marketing & CRM Funnel Integration:** Align outpatient clinic marketing expenditure with patient conversion and actual billing generation.

---

## Dashboard Visual Tour & Storytelling

### 1. High Level Executive Dashboard
<p align="center">
  <img src="./Dashboard%20Previews/High%20Level%20Dashboard.png" alt="Andalusia Healthcare Performance — High Level Dashboard" width="95%">
</p>

---

## Data Architecture & Model
The analytical system utilizes a multi-fact schema connecting clinical billing transactions, medical CRM appointment bookings, and marketing campaign outcomes.

### Model Representation
<p align="center">
  <img src="./Dashboard%20Previews/Model.png" alt="Andalusia Healthcare Performance — Power BI Data Model" width="95%">
</p>

- **Fact Tables:**
  - `fact_billing`: 146 billing records capturing Actual, Baseline, Target, and Historical revenue, volumes, and C/V rates.
  - `fact_medical_crm`: Patient appointment scheduling, attendance, and outpatient volume conversions.
  - `fact_marketing`: Campaign spend, acquisition channels, and conversion efficiency.
- **Dimensions:**
  - `dim_medical_department`: Clinical specialties and diagnostic categories.
  - `dim_bu`: Hospital branches and operational business units.
  - `dim_country`: Regional and national healthcare compliance entities.
  - `dim_payment`: Insurance, corporate contracts, and cash patient payment types.
  - `dim_date`: Calendar dimension enabling fiscal year and monthly run-rate comparisons.

---

## Tools & Technologies
- **Business Intelligence:** Microsoft Power BI Desktop
- **Advanced Calculations:** DAX Target Variance, Realization %, Volume Variance, Cost per Visit Metrics
- **Data Integration:** Multi-source integration across clinical ERP, CRM, and billing logs

---

## License & Usage
This repository is released under the [MIT License](LICENSE). Developed by **Kerelos Nakhla** — Data Analyst & BI Developer.
