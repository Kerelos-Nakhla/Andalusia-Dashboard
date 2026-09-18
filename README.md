# 🏥 ANDALUSIA HEALTHCARE PERFORMANCE — POWER BI

> **Healthcare Performance Analytics | Executive BI Dashboard**

**Andalusia Healthcare Performance** is an interactive **Power BI Business Intelligence solution** developed as a portfolio project based on an interview assessment from **Andalusia Group**.

The project transforms raw healthcare business data into an executive-level analytical experience covering **Billing, Marketing, and CRM** domains. It combines data preparation, Galaxy Schema modeling, Power Query, DAX, and dashboard design to help decision-makers monitor performance, compare actual results against targets and baselines, and identify business trends.

---

## 🖼️ Dashboard Experience

The repository contains the completed Power BI report:

<p align="center">

[![Open Power BI Report](https://img.shields.io/badge/Power%20BI-Open%20Report-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](./3.pbix)

[![Dataset](https://img.shields.io/badge/Excel-Row%20Data-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](./Row%20Data.xlsx)

</p>

> The PBIX file contains the interactive dashboard, data model, Power Query transformations, DAX measures, and report design.

---

## 🎯 Project Objective

The objective was to build a consolidated healthcare performance solution capable of answering questions such as:

- How is overall healthcare performance progressing?
- How does **Actual** performance compare with **Target** and **Baseline**?
- How does current performance compare with **Historical** values?
- Which Business Units contribute to overall performance?
- How does performance vary by Payment Type?
- Where are the strongest and weakest performance areas?
- How can multiple healthcare business domains be brought together into one analytical model?

The result is an executive-oriented BI experience designed to turn operational data into **clear performance indicators and actionable business context**.

---

## 📊 Analytical Scope

| Analytical Area | Purpose |
|---|---|
| 🏥 Billing | Monitor healthcare financial and operational performance |
| 📣 Marketing | Analyze business performance and growth indicators |
| 👥 CRM | Integrate customer-related performance information |
| 🎯 Target | Measure performance against planned objectives |
| 📌 Baseline | Compare current results with baseline values |
| 📚 Historical | Track performance against historical values |
| 🏢 Business Unit | Compare performance across organizational units |
| 💳 Payment Type | Analyze Cash and Credit performance |

---

## 🔎 Data Analysis & Key Insights

### 1. Actual vs Target Performance

The dashboard enables users to compare **Actual performance against Target values**, making it possible to identify achievement levels and performance gaps.

### 2. Actual vs Baseline

Baseline comparisons provide an additional reference point for understanding whether current results are progressing above or below the established benchmark.

### 3. Historical Performance

Historical values provide context for current performance and help users identify changes and growth over time.

### 4. Business Unit Analysis

Performance can be analyzed across **Business Units**, allowing users to move from executive-level KPIs into organizational-level comparisons.

### 5. Payment Type Analysis

The dashboard separates **Cash and Credit** payment behavior, providing another analytical dimension for understanding healthcare performance.

### 6. Integrated Healthcare View

Rather than treating Billing, Marketing, and CRM as isolated datasets, the solution brings them into a unified BI environment through shared dimensions and a Galaxy Schema.

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

**Microsoft Excel** was used during the initial data exploration and preparation stage.

The workflow included:

- Identifying missing values
- Replacing missing values where appropriate
- Reviewing potential outliers
- Checking data consistency
- Preparing the source data for BI analysis

### Power Query

Power Query was used to prepare the data inside Power BI through transformations such as:

- Data type standardization
- Column transformation
- Data cleaning
- Removing unnecessary fields
- Preparing analytical tables

### DAX

DAX measures were developed to support the analytical layer, including:

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

The project uses a **Galaxy Schema** to integrate multiple fact tables around shared analytical dimensions.

### Business Domains

~~~
                  ┌─────────────┐
                  │   Billing   │
                  └──────┬──────┘
                         │
                         │
┌─────────────┐    ┌─────▼─────┐    ┌─────────────┐
│  Marketing  │───►│   Shared  │◄───│     CRM     │
└─────────────┘    │ Dimensions│    └─────────────┘
                   └─────┬─────┘
                         │
                  ┌──────▼──────┐
                  │ Power BI /  │
                  │    DAX      │
                  └─────────────┘
~~~

Shared analytical dimensions include:

- Country
- Business Unit
- Payment Type
- Month

The Galaxy Schema provides a structured foundation for:

- Cross-domain analysis
- Consistent filtering
- Scalability
- Maintainability
- Reusable analytical dimensions

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

Users can interact with the report through:

- Business Unit filtering
- Payment Type filtering
- Country filtering
- Month-level analysis
- Actual vs Target comparisons
- Actual vs Baseline comparisons
- Historical performance comparisons
- Interactive matrix analysis

---

## 🎨 Dashboard Design

The dashboard was designed with an **executive BI perspective**, focusing on clarity, hierarchy, and efficient information consumption.

The design process considered:

- KPI hierarchy
- Visual hierarchy
- Executive readability
- Consistent layout
- Interactive filtering
- Business-oriented storytelling
- Clear comparison between performance benchmarks

The interface was first planned in **Figma** before being implemented in Power BI.

---

## 🧠 Analytical Challenges

### Multi-domain integration

Combining Billing, Marketing, and CRM information required a structured analytical architecture rather than treating each source independently.

### Benchmark comparison

The report needed to distinguish between multiple performance references:

**Actual → Target → Baseline → Historical**

This allows users to understand not only the current result, but also the context around that result.

### Galaxy Schema modeling

The model was designed around shared dimensions so that users can navigate the different business domains through consistent filters.

### Executive communication

The challenge was not only calculating KPIs, but presenting them in a format where performance gaps, trends, and comparisons can be understood quickly.

---

## 🛠️ Technology Stack

| Technology | Role |
|---|---|
| 📊 **Power BI Desktop** | Data modeling, DAX, visualization, and dashboard development |
| 🔄 **Power Query** | Data transformation and preparation |
| 🧮 **DAX** | Measures, KPIs, achievement, and growth calculations |
| 📗 **Microsoft Excel** | Source data exploration and preparation |
| 🎨 **Figma** | Dashboard UI/UX planning |
| 🗂️ **Galaxy Schema** | Analytical data model architecture |

---

## 📁 Repository Structure

~~~
Andalusia-Dashboard/
│
├── 3.pbix
│   └── Power BI report
│
├── Row Data.xlsx
│   └── Source / row-level dataset
│
└── README.md
    └── Project documentation
~~~

---

## 📚 Data Source

The project is based on the data provided for an **Andalusia Group interview assessment**.

The source dataset is included in the repository as:

**[Row Data.xlsx](./Row%20Data.xlsx)**

The Power BI report built from the dataset is included as:

**[3.pbix](./3.pbix)**

---

## 🎓 Project Context

This project demonstrates an end-to-end **Data Analyst / BI Developer** workflow:

**Data Preparation → Data Modeling → Power Query → DAX → Dashboard Design → Business Analysis**

The project focuses on translating business requirements into an analytical solution that allows executives to monitor performance and investigate the context behind it.

---

## 👤 Author

**Kerelos Nakhla Saad**

**Data Analyst | BI Developer**

- GitHub: [Kerelos-Nakhla](https://github.com/Kerelos-Nakhla)
- LinkedIn: [Kerelos Nakhla](https://www.linkedin.com/in/kerelos-nakhla/)

---

## 📌 Repository Files

| File | Description |
|---|---|
| [3.pbix](./3.pbix) | Complete Power BI report |
| [Row Data.xlsx](./Row%20Data.xlsx) | Source row-level dataset |
| [README.md](./README.md) | Project documentation |

---

⭐ **Explore the repository to review the Power BI report, source dataset, analytical model, and dashboard implementation.**
