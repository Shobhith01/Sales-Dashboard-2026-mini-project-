# 📊 Sales Dashboard 2026 — Power BI

<p align="center">
  <img src="https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/DAX-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Mobile%20View-Optimised-blue?style=for-the-badge"/>
</p>

<p align="center">
  An interactive Power BI dashboard built on a retail sales dataset of
  <strong>100 orders across 12 customers in 4 countries</strong> —
  tracking revenue, product performance, and category breakdowns
  using <strong>DAX calculated columns</strong>, table relationships,
  and a custom dark colour theme.
</p>

---

## 📸 Dashboard Preview
 
![Sales Dashboard 2026](dashboard_preview.png)
 
> 🔗 **[View Live Dashboard on Power BI Service](YOUR_PUBLISHED_LINK_HERE)**
> *(Published and optimised for both desktop and mobile view)*
 
---

## 📌 Key Business Findings

| # | Finding | Impact |
|---|---------|--------|
| 1 | **Laptop category dominates** with 51.14% of total revenue ($52.44K) | 🟢 Strongest segment |
| 2 | **Dell XPS 15 is the top product** at $25K — nearly 2× the next product (ThinkPad X1 at $13K) | 🟢 Star performer |
| 3 | **Smartphone is a strong #2** at 23.78% ($24.38K) of total sales | 🟡 Scale opportunity |
| 4 | **Smart Home + Accessory combined = only 6.1%** of total revenue | 🔴 Underperforming segments |
| 5 | All 100 orders spread across just **4 countries** — US, China, Germany, India | 🟡 Geographic concentration risk |
| 6 | **Revenue spike visible in late 2026** — positive growth momentum | 🟢 Upward trend |

---

## 🛠️ Tools & Skills Demonstrated

| Tool / Skill | What Was Done |
|---|---|
| **Power BI Desktop** | Built full interactive dashboard from scratch |
| **DAX — Calculated Columns** | `COALESCE` for null score handling, merged customer name column |
| **Data Modelling** | One-to-many relationship between `customers` and `orders` tables |
| **Power BI Service** | Published report online with shareable live link |
| **Mobile Layout** | Optimised report view for mobile screens |
| **Custom Theme** | Dark colour palette applied manually (`#25201B`, `#FFC300`, `#EA9F00`, `#FFFBFF`) |
| **Interactive Slicers** | Country filter, Product Category filter, Date Range slider |

---

## 📐 DAX Columns Used

```dax
-- Merge first and last name into a single column
customer_name = customers[first_name] & " " & customers[last_name]

-- Handle null scores using COALESCE (replaces nulls with 0)
Clean Score = COALESCE(customers[score], 0)
```

---

## 📊 Dashboard Features

- **3 KPI Cards** — Total Sales ($103K), Total Customers (12), Total Orders (100)
- **Sales Over Time** — Line chart tracking monthly revenue from Jan 2024 to Dec 2026
- **Sales by Product** — Horizontal bar chart of all 19 products ranked by revenue
- **Sales by Category** — Donut chart showing revenue share across 5 product categories
- **3 Interactive Slicers** — Filter by Country, Product Category, and Order Date range
- **Clear All Filters button** — One-click reset for all slicers
- **Mobile layout** — Separate optimised view for phone screens

---

## 🗂️ Project Structure

```
sales-dashboard-powerbi/
│
├── data/
│   ├── customers.csv           # 12 customers — name, country, city, score
│   └── orders.csv              # 100 orders — product, category, quantity, sales
│
├── My_First_Dashboard.pbix     # Power BI Desktop report file
├── dashboard_preview.png       # Full dashboard screenshot
└── README.md
```

---

## 🗃️ Dataset Details

| Field | Details |
|---|---|
| **Orders** | 100 |
| **Customers** | 12 |
| **Countries** | 4 (United States, China, Germany, India) |
| **Product Categories** | 5 (Laptop, Smartphone, Tablet, Smart Home, Accessory) |
| **Products** | 19 unique products |
| **Date Range** | January 2024 — December 2026 |
| **Total Revenue** | $103K |

---

## 🚀 How to Open This Project

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Clone or download this repository
3. Open `My_First_Dashboard.pbix` in Power BI Desktop
4. The data is already embedded — no external connections needed

---

## 🚧 What I'd Improve Next

- [ ] Add Year-over-Year growth DAX measure
- [ ] Include a dedicated customer detail page
- [ ] Add conditional formatting to highlight top/bottom products
- [ ] Expand dataset with more customers and longer date range

---

## 👤 Author

**Shobhith S Kounder**
Aspiring Data Analyst · SQL · Excel · Power BI
📍 Karnataka — Open to relocation anywhere in India

<p>
  <a href="https://www.linkedin.com/in/shobhith-kounder-768859264">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://github.com/Shobhith01">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
</p>

---

<p align="center">
  <i>This is Project 2 of my data analyst portfolio —
  part of a challenge to build job-ready projects in SQL, Excel and Power BI.</i>
</p>
