# Pizza Sales Dashboard

An interactive **Excel dashboard** that analyzes pizza sales for **2015**. It turns raw order data into a clean one-page view of revenue, order volume, and product performance, using pivot tables, pivot charts, slicers, and a date timeline.

![Dashboard preview](<img width="1319" height="476" alt="Pizza Dashboard" src="https://github.com/user-attachments/assets/f2a7e529-3071-42e0-b607-b06d61dcbdc1">)

---

## Key Metrics

| KPI | Value |
|-----|-------|
| Total Sales | $8,436 |
| Total Quantity | 511 |
| Total Orders | 499 |
| Total Customers | 499 |

---

## Dashboard Visuals
<img width="1319" height="476" alt="Pizza Dashboard" src="https://github.com/user-attachments/assets/7bb032e5-b8dc-44e9-8e4e-a5be69ef2d4d" />

| Visual | Chart type | What it shows |
|--------|-----------|---------------|
| Total Sales Per Category | Donut | Share of sales by pizza category (Chicken, Classic, Supreme, Veggie) |
| Sales Distribution By Pizza Size | Pie | Share of sales by size (L, M, S, XL) |
| Monthly Order Volume Peaks | Line | Number of orders per month |
| Weekly Order Distribution | Column | Number of orders per day of the week |
| Top 5 Best-Selling Pizza | Bar | Five pizzas with the highest sales |
| Bottom 5 Least-Selling Pizza | Bar | Five pizzas with the lowest sales |
| Filters | Slicers + Timeline | Pizza size, pizza category, and order date |

---

## Dataset

The `Data` sheet contains one row per order line, with bilingual (Arabic and English) column headers.

| Column | Description |
|--------|-------------|
| `order_date` | Date of the order |
| `WeekDay` | Day of the week |
| `order_time` | Time of the order |
| `unit_price` | Price of one pizza |
| `Sales` | Sales value of the line |
| `pizza_size` | S, M, L, or XL |
| `pizza_category` | Chicken, Classic, Supreme, or Veggie |
| `pizza_ingredients` | List of ingredients |
| `pizza_name` | Name of the pizza |
| `order_id` | Order number |
| `quantity` | Number of pizzas ordered |
| `Customer Name` | Name of the customer |

---

## Workbook Structure

| Sheet | Purpose |
|-------|---------|
| **Data** | The cleaned source data |
| **Pivot Tables** | All pivot tables that feed the charts and KPI cards |
| **Pizza Dashboard** | The final dashboard with KPIs, charts, and slicers |

### Pivot tables used

| Pivot | Rows | Values |
|-------|------|--------|
| Sales by category | `pizza_category` | Sum of Sales (% of total) |
| Sales by size | `pizza_size` | Sum of Sales (% of total) |
| Monthly orders | Month of `order_date` | Count of `order_id` |
| Weekly orders | `WeekDay` | Count of `order_id` |
| Top 5 pizzas | `pizza_name` (Top 5 filter) | Sum of Sales |
| Bottom 5 pizzas | `pizza_name` (Bottom 5 filter) | Sum of Sales |
| KPI cards | None | Sum of Sales, Sum of quantity, Count of `order_id`, Count of Customer Name |

---

## Key Insights

- **Veggie** is the top category by sales (about 28%), followed by Classic (about 27%), Supreme (about 24%), and Chicken (about 21%).
- **Large** pizzas generate almost half of all sales (47%), while XL accounts for only 3%.
- Order volume peaks in **June** (54 orders) and is lowest in **March** (30 orders).
- **Friday** is the busiest day (91 orders) and **Wednesday** is the slowest (48 orders).
- **The Classic Deluxe Pizza** is the best seller ($459), while **The Brie Carre Pizza** sells the least ($47).

---

## Tools & Skills

- **Microsoft Excel**: pivot tables, pivot charts, slicers, timeline
- Data cleaning and preparation
- Dashboard layout and visual design (KPI cards, consistent color theme)

---

## Repository Structure

```
pizza-sales-dashboard/
├── Pizza_Sales_Dashboard.xlsx
├── images/
│   └── dashboard.png
└── README.md
```

---

## How to Use

1. Download or clone this repository.
2. Open `Pizza_Sales_Dashboard.xlsx` in Excel.
3. Go to the **Pizza Dashboard** sheet.
4. Use the **pizza size** and **pizza category** slicers and the **order date** timeline to filter every chart at once.
5. To update the data, edit the **Data** sheet, then click **Data → Refresh All**.

---

## Author

**[Mahmoud Ahmed]**
Technical Translator & Project Support | Data Analytics (Excel, Power Query)
[LinkedIn](https://www.linkedin.com/www.linkedin.com/in/mahmoud-hashem-b8598852) · [Email](mailto:m_translator@ymail.com)
