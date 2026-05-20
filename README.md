# 📊 Sales & Revenue Analysis Dashboard

A fully interactive, single-file sales analytics dashboard built with vanilla HTML, CSS, and JavaScript. Visualize KPIs, revenue trends, top products, and category breakdowns — with support for importing your own CSV or Excel data.

---

## 🖼️ Preview

> Open `sales-dashboard.html` in any modern browser — no installation or build step required.

---

## ✨ Features

- **KPI Cards** — Total Revenue, Total Orders, Average Order Value, and Gross Margin with trend indicators and sparklines
- **Revenue Trend Chart** — Monthly line chart switchable between Revenue, Orders, or both
- **Category Breakdown** — Donut chart showing revenue share across product categories
- **Top Products Chart** — Bar chart of best-performing products by revenue or units sold
- **Top Customers Table** — Ranked by lifetime revenue with visual progress bars
- **Filters & Slicers** — Filter by category, region, and custom date range; all charts update instantly
- **Data Import** — Upload your own `.csv`, `.xlsx`, or `.xls` file and the dashboard remaps automatically
- **Demo Data** — Preloaded with 6 months of sample sales data so it works out of the box

---

## 🚀 Getting Started

### Option 1 — Open Locally
Just download `sales-dashboard.html` and open it in your browser. No server needed.

### Option 2 — Host on GitHub Pages
1. Upload `sales-dashboard.html` to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your dashboard will be live at:
   ```
   https://your-username.github.io/your-repo-name/sales-dashboard.html
   ```

---

## 📂 Importing Your Own Data

Click **Import Data** in the sidebar to load a `.csv`, `.xlsx`, or `.xls` file.

### Expected Column Names
| Column | Accepted Names |
|--------|---------------|
| Date | `date`, `day`, `time` |
| Product | `product`, `item`, `name`, `sku` |
| Category | `category`, `cat`, `type`, `group` |
| Region | `region`, `area`, `zone`, `territory` |
| Units Sold | `units`, `qty`, `quantity`, `count`, `sold` |
| Price / Revenue | `price`, `revenue`, `amount`, `sale`, `total` |
| Cost | `cost`, `cogs`, `expense` |

> Column names are **case-insensitive** and **partial matches** work (e.g. `Unit_Qty` will match `qty`).

### Example CSV Format
```csv
date,product,category,region,units,price,cost
2025-01-05,Wireless Earbuds,Electronics,North,45,79.99,38.00
2025-01-08,Yoga Mat,Sports,West,62,34.99,14.00
```

---

## 🛠️ Built With

| Library | Purpose | Version |
|---------|---------|---------|
| [Chart.js](https://www.chartjs.org/) | All charts and sparklines | 4.4.1 |
| [PapaParse](https://www.papaparse.com/) | CSV file parsing | 5.4.1 |
| [SheetJS (xlsx)](https://sheetjs.com/) | Excel file parsing | 0.18.5 |
| [Syne](https://fonts.google.com/specimen/Syne) | Display / heading font | — |
| [DM Sans](https://fonts.google.com/specimen/DM+Sans) | Body font | — |

All libraries are loaded via CDN — no `npm install` or bundler required.

---


## 📝 License

This project is open source and free to use under the [MIT License](https://opensource.org/licenses/MIT).
