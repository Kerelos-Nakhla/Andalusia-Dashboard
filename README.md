# 🏥 Andalusia Healthcare Performance & Financial Intelligence Dashboard

<p align="center">
  <b>Executive Healthcare Analytics, Outpatient Volume & Revenue Target Tracking in Power BI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/DAX-Financial_Intelligence-blue?style=for-the-badge" alt="DAX" />
  <img src="https://img.shields.io/badge/Healthcare-Clinical_Analytics-green?style=for-the-badge" alt="Healthcare" />
  <img src="https://img.shields.io/badge/Budget_Tracking-Variance_Analysis-critical?style=for-the-badge" alt="Variance Analysis" />
</p>

---

## 📌 Executive Overview
The **Andalusia Healthcare Analytics Dashboard** is an enterprise hospital management and clinical revenue intelligence system built in Power BI for Andalusia Hospitals Group. The dashboard monitors clinical throughput, patient consultation volumes (C/V), baseline expectations, and actual revenue realization across specialized medical departments and geographic business units.

### 📊 Core Key Performance Indicators (KPIs)
- 💵 **Actual Realized Revenue:** **$575,194,957.95** (~$575.2M)
- 🎯 **Target Revenue Budget:** **$724,887,777.62** (~$724.9M)
- 📉 **Budget Target Gap:** **-$149,692,819.67** (20.65% unrealized revenue)
- 📐 **Baseline Revenue Benchmark:** **$706,296,549.89** (~$706.3M)
- ⏳ **Historical Comparative Revenue:** **$463,678,886.83** (~$463.7M)
- 📈 **YoY Revenue Expansion:** **+24.05%** growth over historical baseline
- 🎯 **Budget Achievement Rate:** **79.35%** overall realization rate
- 🩺 **Departmental Coverage:** **146 clinical billing partitions** analyzed across Cardiology, Orthopedics, Pediatrics, Oncology, Internal Medicine, and Surgery

---

## 🎯 Business Problem & Objectives
1. 🔍 **Revenue Target Gap Isolation:** Identify departments lagging behind allocated targets and isolate whether patient volume (consultations) or revenue per visit (C/V) is the root bottleneck.
2. 🏥 **Business Unit Performance Benchmarking:** Compare hospital branches and country operations to allocate clinical staffing and specialized equipment effectively.
3. 📢 **Marketing & Clinical Funnel Alignment:** Connect outpatient clinic marketing spend with patient acquisition, appointment attendance, and actual billing.
4. 🩺 **Specialty Mix Optimization:** Pinpoint high-margin surgical specialties versus high-throughput primary clinics to optimize hospital resource schedules.

---

## 💡 In-Depth Data Analysis & Business Insights
- 📉 **The $149.7M Realization Shortfall:** Realized revenue reached **$575.2M against a $724.9M target (79.35%)**, leaving a 20.65% gap. Although strong YoY growth (+24.05%) occurred, budget targets were set aggressively beyond baseline trends.
- 🩺 **Departmental Variance Drivers:** Over 60% of the budget deficit is concentrated in 4 clinical departments where consultation volume fell below forecasted capacity, despite average revenue per patient remaining stable.
- 🏥 **Branch Operational Disparities:** Top-performing business units achieved 88–92% of target due to integrated diagnostic packages, while secondary branches lagged at 68–74% due to outpatient follow-up drop-offs.
- 🔄 **Marketing vs. Realization Disconnect:** Lead-generating marketing campaigns in select specialties produced high initial inquiry volumes but experienced low conversion to completed consultations.

---

## 🖼️ Dashboard Visual Tour & Storytelling

### 1. High Level Executive Dashboard
<p align="center">
  <img src="./Dashboard%20Previews/High%20Level%20Dashboard.png" alt="Andalusia Healthcare Performance — High Level Dashboard" width="95%">
</p>

---

## 🏗️ Data Architecture & Star Schema
The analytics model integrates clinical, financial, and CRM operations into a unified schema:

- **Fact Tables:**
  - `fact_billing` — Actual outpatient & inpatient billing, transaction dates, departmental IDs, and invoice amounts
  - `fact_marketing` — Campaign expenditures, lead volumes, conversion costs, and channel sources
  - `fact_medical_crm` — Patient inquiries, appointment statuses, attendance confirmation, and cancellations
- **Dimension Tables:**
  - `dim_medical_department` — Clinical specialties (Cardiology, Surgery, Pediatrics, Oncology, Orthopedics, etc.)
  - `dim_bu` — Business units, hospital branches, facility classifications
  - `dim_country` — Geographic regions and national healthcare markets
  - `dim_payment` — Payment methods, insurance providers, self-pay classifications
  - `dim_date` — Fiscal calendar, monthly budget periods, comparative quarters

### 📐 Model Representation
<p align="center">
  <img src="./Dashboard%20Previews/Model.png" alt="Andalusia Healthcare Performance — Power BI Data Model" width="95%">
</p>

---

## 🛠️ Tools & Technologies
- 📊 **Power BI Desktop:** Executive KPI cards, waterfall variance charts, departmental tables
- 📐 **DAX (Data Analysis Expressions):** Budget Achievement %, Target Variance $, Consultation Volume Growth, Cost/Visit (C/V)
- 🧹 **Power Query (M):** Multi-source data merging (Billing ERP + Healthcare CRM + Marketing Logs)
- 🏥 **Domain Modeling:** Healthcare revenue cycle management and outpatient throughput analytics

---

## 📜 License & Author
- **Author:** Kerelos Nakhla ([GitHub](https://github.com/Kerelos-Nakhla))
- **License:** MIT License
