# 📊 Power BI Tools

> A curated collection of professional Power BI dashboards and data analytics projects — built for real-world operations, insights, and decision-making.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

---

## 📁 Repository Structure

```
Power_BI_Tools/
├── 📂 Uber DashBoard/          # Uber Operations Analytics Dashboard (.pbix)
├── 📄 BlinkIT Grocery Data Excel.xlsx   # Source data for BlinkIT grocery analysis
└── 📄 README.md
```

---

## 🚗 Project 1 — Uber Operations Dashboard

A comprehensive Power BI dashboard designed to analyze Uber ride operations and surface actionable insights across **demand, supply, geography, and product performance**.

This project is built to help **operations and city teams** identify peak periods, reduce cancellations, improve driver utilization, and make data-driven decisions at scale.

---

### 🖼️ Dashboard Screenshots

**Overview Page — Executive KPIs**

![Uber Dashboard Overview](https://raw.githubusercontent.com/SatyendraPrajapati456/Power_BI_Tools/main/Uber%20DashBoard/Screenshot%202025-08-19%20204443.png)

> The main overview page shows all critical KPIs at a glance — total trips, driver utilization, completion rate, and more with quick-filter slicers.

---

**Demand & Trend Analysis**

![Demand Trends](https://raw.githubusercontent.com/SatyendraPrajapati456/Power_BI_Tools/main/Uber%20DashBoard/Screenshot%202025-08-19%20204505.png)

> Hourly and weekly seasonality charts with rolling averages and period-over-period comparisons to identify peak demand windows.

---

**Supply & Operations View**

![Supply Operations](https://raw.githubusercontent.com/SatyendraPrajapati456/Power_BI_Tools/main/Uber%20DashBoard/Screenshot%202025-08-19%20204521.png)

> Driver availability, ETA tracking, surge windows, and completion rate breakdown for operational monitoring.

---

**Geography & Cancellations**

![Geography View](https://raw.githubusercontent.com/SatyendraPrajapati456/Power_BI_Tools/main/Uber%20DashBoard/Screenshot%202025-08-19%20205057.png)

> City/zone heatmaps, demand concentration maps, and cancellation trend drill-through diagnostics.

---

### ✨ Features

#### ⏱️ Time Intelligence
- Peak demand analysis by **hour, weekday, and season**
- Trend analysis with **rolling averages** and **period-over-period deltas**

#### 🗺️ Geography & Market Mix
- City/zone performance breakdowns
- **Geo-visuals** (maps and heatmaps) for demand concentration
- Identification of under-served areas

#### 🚦 Supply & Operations
- Driver utilization and wait times
- Completion rate, ETA, and surge window monitoring

#### 🚘 Product Analytics
- Performance by product category (UberX, UberXL, etc.)
- Pricing and promotional effectiveness comparisons

#### 🔁 Quality & Retention
- Cancellation trends and root-cause indicators
- Cohort-style views for repeat ride behavior

---

### 📌 Key KPIs (Metrics)

| KPI | Description |
|---|---|
| 🚗 Total Trips | Overall ride volume |
| 👤 Active Drivers | Supply-side headcount |
| ✅ Completion Rate | Trips completed vs. requested |
| ⏳ Average ETA / Wait Time | Supply efficiency metric |
| ❌ Cancellation Rate | Demand-side friction indicator |
| 💰 Revenue / GMV | Gross monetary value |
| 📦 Trips by Product Type | Category breakdown |
| 🌍 Trips by City/Zone | Geographic segmentation |
| 🕐 Peak Hour / Busiest Day | Time-demand concentration |

---

### 📄 Dashboard Pages

| Page | Content |
|---|---|
| **Overview** | Executive KPIs with quick filters (time, city, product) |
| **Demand Trends** | Hourly/weekly seasonality and growth rates |
| **Supply & Ops** | Driver availability, utilization, wait/ETA, surge |
| **Geography** | City/zone heatmaps, top/bottom performing areas |
| **Product Mix** | Category performance, pricing and promo effects |
| **Cancellations** | Trend analysis and drill-through diagnostics |

**Common Interactions:**
- Cross-highlighting across all charts
- Drill-through from summaries to detail views
- Bookmarks and tooltips for quick narrative context

---

### 🗃️ Data Model

The dashboard uses a **star schema** architecture:

```
Fact Table (Trips)
├── 📅 Dim_Date       → Year, Quarter, Month, Week, Day, Hour, IsWeekend, Season
├── 🌍 Dim_City/Zone  → Geographic hierarchy
├── 🚗 Dim_Product    → Product category (UberX, UberXL, etc.)
├── 👤 Dim_Driver     → Driver attributes
└── 🙋 Dim_Rider      → Rider segmentation
```

- **DAX measures** for KPIs, YoY/PoP comparisons, rolling windows, and segmentation
- **Dedicated Date table** for robust time intelligence

---

### ⚙️ How to Customize

**Add or modify filters:**
> Use _Edit Interactions_ and _Sync Slicers_ in the View tab

**Adjust KPIs:**
> Create or edit DAX measures in the **Model view**

**Add geospatial layers:**
> Ensure latitude/longitude or well-formed geographic fields are present in your data

**Performance tuning:**
> Disable auto-date/time, reduce high-cardinality columns, and use aggregations where needed

---

### 🚀 Performance Tips

- Prefer **numeric surrogate keys** for relationships
- **Summarize granular tables** (e.g., by minute/hour) when appropriate
- Limit expensive **calculated columns** — move logic to Power Query where possible
- Use **incremental refresh** for large historical datasets
- Avoid **bi-directional filters** unless strictly necessary

---

## 🛒 Project 2 — BlinkIT Grocery Data

The repository also includes `BlinkIT Grocery Data Excel.xlsx` — a structured dataset for grocery analytics, suitable for building inventory, sales, and outlet performance dashboards in Power BI.

**Potential use cases:**
- Outlet-level sales performance
- Product category and fat content analysis
- Item visibility vs. sales correlation
- Tier-wise location performance

---

## 🛠️ Requirements

- **Power BI Desktop** (latest version recommended)
- **Microsoft Excel** (for `.xlsx` data source)
- Basic understanding of DAX and Power Query (for customization)

---

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/SatyendraPrajapati456/Power_BI_Tools.git
   ```

2. **Open the `.pbix` file** in Power BI Desktop

3. **Connect your data source** or explore the dashboard with sample data

4. **Customize** KPIs, slicers, and layouts to match your use case

5. **Publish** to Power BI Service for team sharing

---

## 👤 Author

**Satyendra Prajapati**
- GitHub: [@SatyendraPrajapati456](https://github.com/SatyendraPrajapati456)

---

## 📜 License

This project is open for learning and personal use. Please credit the author if you build upon these dashboards.

---

> ⭐ **If this project helped you, give it a star!** It motivates continued improvements and new dashboard additions.
