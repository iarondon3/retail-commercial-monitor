# 📂 Data

## Dataset: `transactions_clean.xlsx`

Clean retail transactions dataset containing **25,000 records** spanning from **January 2024 to February 2026**.

---

## 📋 Column Dictionary

| Column | Type | Description |
|--------|------|-------------|
| `date` | Date | Transaction date |
| `order_id` | Integer | Unique order identifier |
| `customer_id` | Integer | Unique customer identifier |
| `region` | String | Sales region (Norte, Sur, Este, Oeste) |
| `channel` | String | Sales channel (Online, Retail) |
| `category` | String | Product category (Electrónica, Hogar, Deportes, Oficina) |
| `product` | String | Product name |
| `qty` | Integer | Units sold per transaction |
| `unit_price` | Float | Price per unit before discount |
| `discount` | Float | Discount rate applied (0 to 1) |
| `revenue` | Float | Total revenue after discount |
| `cost` | Float | Total cost of goods sold |
| `returned` | Integer | Whether the order was returned (1 = Yes, 0 = No) |
| `ship_days` | Float | Days from order to shipment |
| `year` | Integer | Transaction year |
| `month` | Integer | Transaction month |
| `year_month` | Date | Year-month grouping for time series |
| `week` | Integer | Week number of the year |
| `profit` | Float | Revenue minus cost |
| `margin` | Float | Profit margin (profit / revenue) |
| `revenue_outlier` | Boolean | Flags transactions with abnormally high revenue |

---

## 🔍 Key Stats

| Metric | Value |
|--------|-------|
| Total records | 25,000 |
| Time period | Jan 2024 – Feb 2026 |
| Regions | 4 (Norte, Sur, Este, Oeste) |
| Channels | 2 (Online, Retail) |
| Categories | 4 (Electrónica, Hogar, Deportes, Oficina) |
| Unique products | 20+ |

---

## ⚠️ Known Data Quality Issue

A small segment of transactions contains **"Desconocido" (Unknown)** as the product name, indicating incomplete SKU mapping at the point of entry. This is documented as **Insight 3** in the main analysis — see the project [README](../README.md) for details.
