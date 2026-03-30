# 📊 Power BI Tools

> A curated collection of professional **Power BI dashboards** and real-world data analytics projects — designed to surface actionable insights for operations, retail, and city teams.

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white"/>
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white"/>
  <img src="https://img.shields.io/badge/Power%20Query-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge"/>
</p>

---

## 📁 Repository Structure

```
Power_BI_Tools/
│
├── 📂 Uber DashBoard/                      # Uber Ride Operations Dashboard (.pbix + screenshots)
│   ├── 📊 Uber Dashboard.pbix
│   ├── 🖼️ <img width="1290" height="731" alt="Screenshot 2026-03-30 231702" src="https://github.com/user-attachments/assets/9e97d654-dea4-4247-a7c8-762d39b0e2db" />
  # Overview KPIs
│   ├── 🖼️ <img width="1290" height="731" alt="Screenshot 2026-03-30 231702" src="https://github.com/user-attachments/assets/1e606e80-60bd-4b06-b465-2029afe90a20" />
 # Demand & Trends
│   ├── 🖼️ <img width="1292" height="731" alt="Screenshot 2026-03-30 231748" src="https://github.com/user-attachments/assets/0b1655f7-48c4-4148-b315-39d4e70a472e" />
  # Supply & Ops / Customization
│   └── 🖼️ <img width="1293" height="732" alt="Screenshot 2026-03-30 231719" src="https://github.com/user-attachments/assets/bf2f0de4-9803-43cc-abe6-599b8fa3b690" />
  # Geography & Performance
│
└── 📄 README.md
```

---

## 🚗 Project 1 — Uber Operations Dashboard

A comprehensive **Power BI dashboard** built to analyze Uber ride operations and surface actionable insights across demand, supply, geography, and product performance.

This project empowers **operations teams and city managers** to:
- Identify peak demand windows 🕐
- Reduce cancellations and improve rider experience ❌➡️✅
- Optimize driver utilization 🚗
- Make data-driven operational decisions 📈

---

### 🖼️ Dashboard Screenshots

---

#### 🔹 Overview — Executive KPIs

![Uber Dashboard Overview](https://github.com/SatyendraPrajapati456/Power_BI_Tools/blob/main/Uber%20DashBoard/Screenshot%202025-08-19%20204443.png?raw=true)

> The main overview page presents all critical KPIs at a glance — total trips, active drivers, completion rate, cancellation rate, and revenue — with quick-filter slicers for time, city, and product type.

---

#### 🔹 Demand & Trend Analysis

![Demand Trends](https://github.com/SatyendraPrajapati456/Power_BI_Tools/blob/main/Uber%20DashBoard/Screenshot%202025-08-19%20204505.png?raw=true)

> Hourly and weekly seasonality charts with rolling averages and period-over-period comparisons to identify peak demand windows and growth trends.

---

#### 🔹 Supply, Operations & Customization

![Supply and Operations](https://github.com/SatyendraPrajapati456/Power_BI_Tools/blob/main/Uber%20DashBoard/Screenshot%202025-08-19%20204521.png?raw=true)

> Driver availability, ETA tracking, surge window monitoring, and completion rate breakdowns — plus how to add/modify filters using Edit Interactions and Sync Slicers.

---

#### 🔹 Geography, Performance & Cancellations

![Geography and Cancellations](https://github.com/SatyendraPrajapati456/Power_BI_Tools/blob/main/Uber%20DashBoard/Screenshot%202025-08-19%20205057.png?raw=true)

> City/zone heatmaps, demand concentration maps, top/bottom performing areas, and cancellation trend drill-through diagnostics.

---

### ✨ Features

| Category | Details |
|---|---|
| ⏱️ **Time Intelligence** | Peak demand by hour, weekday & season; rolling averages; YoY/PoP deltas |
| 🗺️ **Geography & Market Mix** | City/zone performance; geo-visuals (maps & heatmaps); under-served area detection |
| 🚦 **Supply & Operations** | Driver utilization, wait times, completion rate, ETA, surge windows |
| 🚘 **Product Analytics** | UberX, UberXL & other categories; pricing & promo effectiveness |
| 🔁 **Quality & Retention** | Cancellation trend analysis; cohort-style repeat rider views |

---

### 📌 Key KPIs

| KPI | Description |
|---|---|
| 🚗 Total Trips | Overall ride volume across all cities and product types |
| 👤 Active Drivers | Supply-side headcount — drivers who completed at least one trip |
| ✅ Completion Rate | % of requested trips that were successfully completed |
| ⏳ Average ETA / Wait Time | Key supply efficiency indicator for rider satisfaction |
| ❌ Cancellation Rate | Demand-side friction — segmented by reason and city |
| 💰 Revenue / GMV | Gross monetary value across all product types |
| 📦 Trips by Product Type | Category-level volume breakdown |
| 🌍 Trips by City/Zone | Geographic segmentation for market-level views |
| 🕐 Peak Hour / Busiest Day | Demand concentration by time dimension |

---

### 📄 Dashboard Pages

| Page | What You'll Find |
|---|---|
| **Overview** | Executive KPIs with quick filters — time, city, product |
| **Demand Trends** | Hourly/weekly seasonality, growth rates, rolling averages |
| **Supply & Ops** | Driver availability, utilization, wait/ETA, surge windows |
| **Geography** | City/zone heatmaps, top and bottom performing areas |
| **Product Mix** | Category performance, pricing and promotional effects |
| **Cancellations** | Trend analysis with drill-through diagnostics |

**Common Interactions:**
- Cross-highlighting across all visuals
- Drill-through from summary views to granular detail
- Bookmarks and dynamic tooltips for quick narrative context

---

### 🗃️ Data Model (Star Schema)

```
Fact Table: Trips
├── 📅 Dim_Date       → Year, Quarter, Month, Week, Day, Hour, IsWeekend, Season
├── 🌍 Dim_City/Zone  → Geographic hierarchy and tier classification
├── 🚗 Dim_Product    → Product category (UberX, UberXL, Pool, etc.)
├── 👤 Dim_Driver     → Driver attributes and segment
└── 🙋 Dim_Rider      → Rider cohort and retention segment
```

- **DAX measures** covering KPIs, YoY/PoP comparisons, rolling windows, and cohort segmentation
- **Dedicated Date table** with full time intelligence support (fiscal, calendar, seasonal)

---

### ⚙️ How to Customize

**🔧 Add or modify filters**
> Use *Edit Interactions* and *Sync Slicers* in the View ribbon to control cross-filter behavior.

**📐 Adjust KPIs**
> Create or edit DAX measures in **Model view** → New Measure.

**🗺️ Add geospatial layers**
> Ensure your data includes latitude/longitude or well-formed geographic hierarchy columns.

**⚡ Performance tuning**
> Disable auto-date/time, reduce high-cardinality columns, and leverage aggregations where possible.

---

### 🚀 Performance Best Practices

- Prefer **numeric surrogate keys** for all table relationships
- **Summarize high-granularity tables** (e.g., minute-level → hour-level) when full grain isn't needed
- Keep **calculated columns minimal** — push logic to Power Query (M) for better performance
- Use **incremental refresh** for large historical trip datasets
- Avoid **bi-directional filters** unless strictly required by the report logic

---

## 🛒 Project 2 — BlinkIT Grocery Analytics Data

The repository includes **`BlinkIT Grocery Data Excel.xlsx`** — a structured, ready-to-use dataset for building grocery retail analytics dashboards in Power BI.

### Dataset Highlights

| Field Category | Examples |
|---|---|
| 📦 Product Info | Item name, type, fat content, category |
| 🏪 Outlet Info | Outlet ID, size, location tier, establishment year |
| 💵 Sales Metrics | Item sales, item visibility, item MRP (price) |
| ⭐ Ratings | Customer rating per outlet-item combination |

### Potential Dashboard Use Cases

- **Outlet-level sales performance** — Which outlets drive the most revenue?
- **Product category analysis** — Which item types sell best?
- **Fat content breakdown** — Regular vs. low-fat product performance
- **Item visibility vs. sales** — Does shelf visibility drive conversions?
- **Tier-wise location performance** — Tier 1 vs. Tier 2 vs. Tier 3 city comparison
- **Outlet age analysis** — Does establishment year affect sales?

---

## 🛠️ Requirements

| Tool | Purpose |
|---|---|
| **Power BI Desktop** (latest) | Open and edit `.pbix` dashboard files |
| **Microsoft Excel** | View/edit the `.xlsx` source data |
| **DAX knowledge** (basic) | Customize existing measures and KPIs |
| **Power Query knowledge** (basic) | Modify data transformation steps |

---

## 🚀 Getting Started

```bash
# 1. Clone this repository
git clone https://github.com/SatyendraPrajapati456/Power_BI_Tools.git

# 2. Navigate into the project folder
cd Power_BI_Tools
```

Then:
1. Open `Uber DashBoard/` → double-click the `.pbix` file to open in **Power BI Desktop**
2. **Explore** the dashboard using built-in sample data
3. **Connect your own data source** by updating the data source settings in Transform Data
4. **Customize** KPIs, visuals, and slicers to suit your use case
5. **Publish** to Power BI Service to share with your team

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve an existing dashboard or add a new one:

1. Fork this repository
2. Create a new branch (`git checkout -b feature/new-dashboard`)
3. Commit your changes
4. Open a Pull Request with a description of what you've added

---

## 👤 Author

**Satyendra Prajapati**
- 🔗 GitHub: [@SatyendraPrajapati456](https://github.com/SatyendraPrajapati456)

---

## 📜 License

This project is open for learning and personal use. Please credit the original author if you build upon or share these dashboards.

---

<p align="center">
  ⭐ <strong>Found this useful? Give it a star!</strong> It encourages continued improvements and new dashboard additions. ⭐
</p>
