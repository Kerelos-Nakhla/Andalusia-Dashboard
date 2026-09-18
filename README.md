# 🏥 ANDALUSIA HEALTHCARE PERFORMANCE — POWER BI

> **Healthcare Performance Analytics | Executive BI Dashboard**

**Andalusia Healthcare Performance** is an interactive **Power BI Business Intelligence solution** developed as a portfolio project based on an interview assessment from **Andalusia Group**.

The project transforms healthcare business data into an executive-level analytical experience covering **Billing, Marketing, and CRM**. It combines data preparation, Galaxy Schema modeling, Power Query, DAX, Figma-based dashboard design, and interactive Power BI reporting.

---

## 🖼️ Dashboard Experience

### High-Level Dashboard

<p align="center"><img src="./Screenshots/High%20Level%20Dashboard.png" alt="Andalusia Healthcare Performance — High Level Dashboard" width="900"></p>

### Data Model

<p align="center"><img src="./Screenshots/Model.png" alt="Andalusia Healthcare Performance — Galaxy Schema Data Model" width="900"></p>

---

## 🎯 Project Objective

The objective was to build a consolidated healthcare performance solution capable of answering questions such as:

- How is overall healthcare performance progressing?
- How does **Actual** performance compare with **Target** and **Baseline**?
- How does current performance compare with **Historical** values?
- Which Business Units contribute to overall performance?
- How does performance vary by Payment Type?
- How does healthcare performance change over time?
- How can Billing, Marketing, and CRM data be integrated into one analytical model?

The result is an executive-oriented BI experience designed to turn operational data into **clear KPIs, comparisons, trends, and business context**.

---

## 📊 Data at a Glance

The repository now contains a structured analytical dataset with **8 Excel tables**:

| Type | Tables | Count |
|---|---|---:|
| 📐 Dimensions | Business Unit, Country, Date, Medical Department, Payment | **5** |
| 📊 Facts | Billing, Marketing, Medical CRM | **3** |
| 🗂️ Total analytical tables | Dimensions + Facts | **8** |

### Analytical domains

| Domain | Dataset |
|---|---|
| 🏥 Billing | fact_billing.xlsx |
| 📣 Marketing | fact_marketing.xlsx |
| 👥 Medical CRM | fact_medical_crm.xlsx |

### Shared dimensions

- dim_bu.xlsx — Business Units
- dim_country.xlsx — Countries
- dim_date.xlsx — Date / time analysis
- dim_medical_department.xlsx — Medical departments
- dim_payment.xlsx — Payment types

> **Data note:** The repository structure was verified directly from the current GitHub dataset. Exact row-level KPI totals are intentionally not hard-coded here until the binary Excel workbooks can be read reliably.

---

## 🔎 Business Analysis

### 1. Actual vs Target

The dashboard compares actual performance with defined targets, allowing users to evaluate **achievement and performance gaps** rather than looking at absolute values alone.

### 2. Actual vs Baseline

Baseline comparison provides a second benchmark for understanding whether performance is above or below the established reference point.

### 3. Historical Performance

The dedicated date dimension enables performance to be analyzed over time and compared with historical values.

### 4. Business Unit Analysis

The Business Unit dimension allows users to move from executive KPIs into organizational-level performance analysis.

### 5. Payment Type Analysis

Payment types provide an additional financial/business dimension, including the project's **Cash vs Credit** analysis.

### 6. Medical Department Analysis

The medical department dimension enables healthcare performance to be investigated across different clinical/business areas.

### 7. Cross-domain Analysis

The three fact domains — **Billing, Marketing, and Medical CRM** — are brought together through shared dimensions, allowing consistent filtering and analysis across the model.

---

## 🔄 End-to-End BI Workflow

~~~
Raw Healthcare Data
        ↓
Excel Data Exploration
        ↓
Data Cleaning & Validation
        ↓
Power Query
        ↓
Galaxy Schema Data Model
        ↓
DAX Measures
        ↓
Power BI
        ↓
Interactive Executive Dashboard
        ↓
Business Performance Analysis
~~~

### Data Preparation

The source data was explored and prepared before being modeled in Power BI.

The preparation workflow included:

- Identifying missing values
- Reviewing data consistency
- Reviewing potential outliers
- Standardizing analytical fields
- Preparing data for modeling

### Power Query

Power Query was used for:

- Data type standardization
- Data transformation
- Data cleaning
- Removing unnecessary fields
- Preparing analytical tables

### DAX

DAX measures were developed for analytical KPIs including:

- Actual
- Target
- Baseline
- Historical
- Achievement %
- Growth %
- Revenue KPIs
- Operational KPIs

---

## 🗂️ Data Model

The project uses a **Galaxy Schema**, with multiple fact tables connected through shared dimensions.

### Model Structure

~~~
                    ┌────────────────────┐
                    │    dim_date        │
                    └─────────┬──────────┘
                              │
┌──────────────┐     ┌────────▼─────────┐     ┌──────────────┐
│   dim_bu     │────►│ Shared Dimensions│◄────│ dim_country  │
└──────────────┘     └────────┬─────────┘     └──────────────┘
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
   ┌──────▼──────┐     ┌──────▼──────┐     ┌──────▼─────────┐
   │fact_billing │     │fact_marketing│    │fact_medical_crm│
   └─────────────┘     └─────────────┘     └────────────────┘
~~~

Additional shared dimensions include:

- Medical Department
- Payment Type

This architecture supports:

- Cross-domain analysis
- Consistent filtering
- Reusable dimensions
- Scalability
- Maintainability
- Clear separation of analytical grain

---

## 📈 Dashboard Features

### Executive KPIs

The dashboard provides KPI-level visibility into:

- Actual
- Target
- Baseline
- Historical
- Achievement %
- Growth %

### Interactive Analysis

Users can analyze the report through:

- Business Unit filtering
- Country filtering
- Payment Type filtering
- Medical Department filtering
- Month/date analysis
- Actual vs Target comparison
- Actual vs Baseline comparison
- Historical performance comparison
- Interactive matrix analysis

---

## 🎨 Dashboard Design

The dashboard was designed from an **executive BI perspective**, focusing on information hierarchy and efficient decision support.

The design process considered:

- KPI hierarchy
- Visual hierarchy
- Executive readability
- Consistent layout
- Interactive filtering
- Business-oriented storytelling
- Clear benchmark comparisons

**Figma** was used during the dashboard design stage before implementation in Power BI.

---

## 🧠 Analytical Challenges

### Multi-domain integration

Billing, Marketing, and Medical CRM have different analytical purposes. The Galaxy Schema provides a common structure for analyzing them through shared dimensions.

### Multiple performance benchmarks

The dashboard distinguishes between:

**Actual → Target → Baseline → Historical**

This makes it possible to evaluate current performance from several business perspectives.

### Time-based analysis

The dedicated date dimension supports period-based analysis and historical comparisons.

### Executive communication

The challenge was not only to calculate KPIs, but to present them in a format where performance, gaps, and trends can be understood quickly.

---

## 🛠️ Technology Stack

| Technology | Role |
|---|---|
| 📊 **Power BI Desktop** | Data modeling, visualization, and dashboard development |
| 🔄 **Power Query** | Data transformation and preparation |
| 🧮 **DAX** | Dynamic measures and KPI calculations |
| 📗 **Microsoft Excel** | Source data and analytical tables |
| 🎨 **Figma** | Dashboard UI/UX planning |
| 🗂️ **Galaxy Schema** | Analytical data model architecture |

---

## 📁 Repository Structure

~~~
Andalusia-Dashboard/
│
├── Andalusia.pbix
│   └── Complete Power BI report
│
├── Dataset/
│   ├── dim_bu.xlsx
│   ├── dim_country.xlsx
│   ├── dim_date.xlsx
│   ├── dim_medical_department.xlsx
│   ├── dim_payment.xlsx
│   ├── fact_billing.xlsx
│   ├── fact_marketing.xlsx
│   └── fact_medical_crm.xlsx
│
├── Screenshots/
│   ├── High Level Dashboard.png
│   └── Model.png
│
└── README.md
~~~

---

## 📚 Data Source

The project is based on data provided for an **Andalusia Group interview assessment**.

The cleaned analytical tables are included in the repository under the **Dataset** folder.

The Power BI report is included as:

**[Andalusia.pbix](./Andalusia.pbix)**

---

## 🎓 Project Context

This project demonstrates an end-to-end **Data Analyst / BI Developer** workflow:

**Data Preparation → Data Modeling → Power Query → DAX → Dashboard Design → Business Analysis**

The project focuses on translating business requirements into an analytical solution that allows executives to monitor performance, compare benchmarks, investigate trends, and explore different business dimensions.

---

## 👤 Author

**Kerelos Nakhla Saad**

**Data Analyst | BI Developer**

- GitHub: [Kerelos-Nakhla](https://github.com/Kerelos-Nakhla)
- LinkedIn: [Kerelos Nakhla](https://www.linkedin.com/in/kerelos-nakhla/)

---

## 📌 Repository Files

| File / Folder | Description |
|---|---|
| [Andalusia.pbix](./Andalusia.pbix) | Complete Power BI report |
| [Dataset](./Dataset) | Structured analytical Excel tables |
| [Screenshots](./Screenshots) | Dashboard and data-model screenshots |
| [README.md](./README.md) | Project documentation |

---

⭐ **Explore the repository to review the dashboard, data model, analytical tables, and complete Power BI implementation.**
