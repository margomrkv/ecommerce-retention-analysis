# E-commerce Retention Analysis

**Author:** [Margarita Markova](https://github.com/margomrkv)

Final project for **Product Analytics** module at [Karpov Courses](https://karpov.courses/).

**Business question:** Why isn't marketplace revenue growing, and what should the product team do?

Analysis performed on the public dataset from Brazilian marketplace **[Olist](https://olist.com/)** — real e-commerce data (~100k orders, 2016–2018).

---

## About

The marketplace has stalled revenue growth for several months. The goal is to identify the product issue and propose measurable actions without degrading user experience.

**Analysis focus:** orders and buyer behavior after first purchase — retention, repeat orders, **GMV** (Gross Merchandise Value), cancellations.

**Methods:** cohort retention analysis, product/market fit assessment, product metrics, hypothesis prioritization (ICE framework), recommendations for product team.

---

## What I Did

**Problem:** Brazilian e-commerce startup — revenue stagnant for months. Need to find the cause and propose a solution.

- Monthly retention cohort analysis at order placement stage
- Product/market fit assessment from behavioral data
- Identified 5 key metrics for profit maximization
- Hypothesis prioritization using ICE framework
- Defined target, proxy, and guardrail metrics for selected hypothesis

**Key findings:**
- **No PMF:** users make one purchase and don't return; retention curve never plateaus
- **Top priority (ICE score: 192):** fix bug in order processing system
- **Scaling and new markets not viable** until retention reaches ≥5%

Full analysis, charts, and calculations in [`ecommerce_retention_analysis.ipynb`](./ecommerce_retention_analysis.ipynb).

---

## Stack

- **Python 3.10+**
- **pandas**, **numpy**
- **matplotlib**, **seaborn** — cohort heatmaps, metrics dynamics
- **statsmodels** — z-test for proportion comparison between cohorts

---

## Repository Structure

```
.
├── README.md
├── LICENSE
├── requirements.txt
├── ecommerce_retention_analysis.ipynb
├── olist_customers_dataset.csv
├── olist_orders_dataset.csv
└── olist_order_items_dataset.csv
```

---

## Data

Three tables from the public **[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)** (Kaggle). Source: Brazilian marketplace [Olist](https://olist.com/), period **2016–2018**.

| File | Content |
|------|---------|
| `olist_customers_dataset.csv` | Customers |
| `olist_orders_dataset.csv` | Orders (statuses, dates) |
| `olist_order_items_dataset.csv` | Order items (price, product) |

Project code is distributed under [MIT License](./LICENSE); data usage governed by [Kaggle dataset terms](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

---

## Contact

GitHub: [@margomrkv](https://github.com/margomrkv)

---

*Last updated: 2026-06-29*
