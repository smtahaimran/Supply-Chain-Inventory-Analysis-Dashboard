# Supply Chain & Inventory Analysis Dashboard

A project analyzing a full year of ordering, delivery, and inventory data for a 6-store bakery chain, built to identify why ingredients keep running out, which suppliers are actually reliable, and how much stockouts and spoilage are costing the business.

---

## 📌 Project Overview

**Client brief:** Sweet Crust Bakery operates six stores across Lahore, Karachi, Islamabad, and Rawalpindi. Some stores kept running out of key ingredients while others overstocked, there was no clear way to track supplier reliability, and nobody had a clear picture of how much money was being lost to spoiled stock and missed sales.

**Goal:** Turn a full year of raw inventory and purchase order data into a Power BI dashboard and a client-ready report identifying the root causes and recommending specific, actionable fixes.

---

## 🗂️ Dataset

The analysis combines five linked datasets covering a full year (Jan–Dec 2025):

| File | Description | Rows |
|---|---|---|
| `dim_stores.csv` | The 6 bakery store locations | 6 |
| `dim_products.csv` | 12 core ingredients across 4 categories (Dry Goods, Dairy, Baking Essentials, Perishables) | 12 |
| `dim_suppliers.csv` | 6 suppliers with lead time and reliability data | 6 |
| `fact_inventory_daily.csv` | Daily stock levels, usage, wastage, and stockouts per store/product | 26,280 |
| `fact_purchase_orders.csv` | Purchase orders with delivery timing, quantities, and cost | 3,141 |

The data is synthetic but statistically modeled to behave like a real bakery's operations — including Pakistan-specific seasonal demand patterns (Ramadan, Eid-ul-Fitr, Eid-ul-Adha, winter wedding season), weekend demand spikes, shelf-life-driven spoilage, and supplier-specific delivery reliability.

---

## 📊 Dashboard

The dashboard has 6 report pages, each with 4 focused visuals:

1. **Executive Overview** — spend, stockout rate, on-time delivery vs. target, demand trend
2. **Inventory & Stockouts** — stockout rate by store/product, lost sales value
3. **Wastage & Spoilage** — spoilage cost by product, store, and category
4. **Supplier Performance** — on-time delivery %, fill rate, lead time reliability
5. **Demand & Seasonality** — Ramadan/Eid/wedding season demand patterns
6. **Cost & Spend Analysis** — spend breakdown by category, supplier, and store
7. **Key Insights**
8. **Recommendations**


---

## 🔑 Key Insights

- Only **55% of supplier deliveries arrive on time**, well below a healthy 90% target (the leading driver of stockouts across the business).
- **Perishable ingredients stock out ~28% of the time**, compared to under 5% for dairy and almost never for dry goods (the stockout problem is fundamentally about shelf life, not poor planning overall).
- **Fresh Strawberries are the single biggest stockout risk**, driven by limited off-season (Jun–Oct) supply rather than under-ordering.
- **Stockouts and wastage together cost an estimated PKR 4.39 million** over the year (PKR 4M in lost sales, PKR 388K in spoilage) — against PKR 147.6M in total spend.
- **Two stores (Gulberg and Satellite Town) drive a disproportionate share of chain-wide stockouts**, making them the natural starting point for fixes.
- Demand spikes predictably during **Ramadan/Eid** and the **winter wedding season (Nov–Feb)**, and is consistently **15–35% higher on weekends**.

---

## ✅ Recommendations

- Renegotiate delivery schedules or hold extra safety stock for suppliers with poor on-time performance.
- Order perishables (strawberries, milk, butter, cream cheese) more frequently and in smaller batches.
- Source a second supplier for strawberries to cover the June–October off-season.
- Prioritize Gulberg and Satellite Town when piloting ordering changes before rolling out chain-wide.
- Build seasonal stock buffers ahead of Ramadan, Eid, and wedding season.
- Score suppliers separately on delivery timing and order completeness, since they're two distinct problems.
---
