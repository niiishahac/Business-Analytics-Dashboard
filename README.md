# Business-Analytics-Dashboard
project on power bi
# 📊 Business Analytics Dashboard — Power BI

An interactive business analytics dashboard built in Power BI, integrating multiple data sources through Power Query and DAX to deliver real-time visual insights across sales, products, regions, and customers.

---

## 🖼️ Dashboard Preview

> *Open the `.pbix` file in Power BI Desktop to explore the fully interactive dashboard.*

---

## 🚀 Features

- **KPI Cards** — Real-time metrics for Total Revenue, Target, Gross Margin, and Orders
- **Monthly Trend Chart** — Clustered bar + line combo showing Revenue vs Target across 12 months
- **Donut Chart** — Category-wise revenue breakdown (Software, Hardware, Services, Consulting)
- **Region Slicer** — Interactive tile-style filter (North / South / East / West) with cross-filtering across all visuals
- **Products Table** — Conditional formatting with color-coded margin performance (Green / Yellow / Red)

---

## 🗂️ Data Sources

| Table | Description |
|-------|-------------|
| `Sales` | Monthly revenue, target, gross margin, and orders |
| `Products` | Product-level revenue, margin %, category, and status |
| `Regions` | Regional revenue, targets, and attainment % |
| `Customers` | 50 customers with orders, spend, and segments |

---

## 🧮 DAX Measures

```dax
Total Revenue = SUM(Sales[Revenue])

Gross Margin % = AVERAGE(Sales[Gross_Margin])

Avg Order Value = DIVIDE([Total Revenue], [Total Orders])

Attainment % = DIVIDE([Total Revenue], [Revenue Target])

Active Customers = DISTINCTCOUNT(Customers[Customer_ID])
```

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Dashboard design and visualization |
| **Power Query** | Data transformation and cleaning |
| **DAX** | Calculated measures and KPIs |
| **Microsoft Excel** | Source data (.xlsx) |

---




