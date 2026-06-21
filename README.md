# Brazilian E-Commerce — Sales & Delivery Performance Pipeline
**Author:** Fariba Kazi

An end-to-end analytics pipeline on 100K+ Brazilian e-commerce orders — moving raw data through Excel, Python, SQL, and Power BI to answer a real business question.

## Business Question
Which product categories, regions, and sellers drive the most revenue — and where is delivery performance hurting customer satisfaction?

## Pipeline
**Excel** (profiling) → **Python / pandas** (cleaning + joining 7 tables) → **SQL / SQLite** (validation queries) → **Power BI** (dashboard)

## Dataset
[Brazilian E-Commerce Public Dataset by Olist (Kaggle)](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) — 9 tables, 100K+ orders (2016–2018).

## Key Findings
1. **Top categories:** Health & Beauty (BRL 1.26M), Watches & Gifts (BRL 1.20M), and Bed/Bath/Table (BRL 1.04M) lead revenue.
2. **Regional concentration:** São Paulo dominates customers (about 42%) and revenue (BRL 5.2M, nearly 3x the next state); the top 3 states are all in the Southeast.
3. **Seller concentration:** Of 3,095 sellers, the top 10 (0.3%) drive about 13% of revenue.
4. **Delivery drives satisfaction:** On-time orders average around 4.2 stars vs around 2.3 for late orders — late delivery nearly halves the score, and only about 7% of orders are late.

## Dashboard
![Dashboard](ecommerce_pipeline_dashboard.jpg)

*Built in Power BI — revenue by category, revenue by region, top sellers, review score by delivery status, plus total-revenue and average-delivery-time KPIs.*

## Recommendation
Delivery reliability is the highest-leverage fix: a small share of late orders does outsized damage to satisfaction. Tightening logistics or setting more realistic delivery estimates would protect reviews and retention.

## Process
Profiled raw tables in Excel, then in Python cleaned missing values, engineered delivery metrics, fixed a duplicate-reviews join issue, and joined 7 tables into an analysis-ready dataset. Validated findings with SQL (aggregations and joins), then visualized in Power BI.

## Tools
Excel · Python (pandas) · SQL (SQLite) · Power BI
