<h1 align="center">Hi, I'm Calvince Okoth 👋</h1>
<h3 align="center">Data Analyst · Aspiring Data Engineer · Nairobi, Kenya</h3>

<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/SQL-0b7bb5?style=for-the-badge&logo=mysql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
</p>

<p align="center">
  <a href="https://claude.ai/artifact/2ZyVQsxFbK4AmPrFA2dydM"><b>Portfolio</b></a> ·
  <a href="https://www.linkedin.com/in/calvince-okoth-85792b25a/"><b>LinkedIn</b></a> ·
  <a href="mailto:calvinceokoth59@gmail.com"><b>Email</b></a> ·
  <a href="https://wa.me/254703161063"><b>WhatsApp</b></a>
</p>

---

## About me

I turn raw data into decisions a business can act on. I work with PostgreSQL, SQL, Excel and Power BI, and I come from a background in data annotation, quality assurance and structured data review, so I check my data carefully before I trust any number.

I am open to **data analyst** and **junior data engineer** roles, and to collaborating on data projects.

## How I work

1. **Understand** the business question and the decision it supports.
2. **Validate** row counts, keys and dates before trusting any result.
3. **Analyse** with clear, readable SQL and documented business rules.
4. **Recommend** one clear action for management.

## Featured projects

### 📊 [Duka Smart Electronics: Retail Sales & Customer Analytics](https://github.com/Calvincekoth/retail-sales-sql)
A PostgreSQL project for a fictional Kenyan electronics retailer. I built the database, validated the data and answered 46 business questions on customer value, product profitability, sales momentum and inactivity.

| Completed revenue | Gross margin | Orders analysed | SQL queries |
|:---:|:---:|:---:|:---:|
| KSh 24.2M | 12.0% | 800 | 46 |

**Key findings**
- Discounts create losses: 62 order lines sold below cost, about KSh −142k, mostly on refrigerators, TVs and phones.
- Accessories win on margin: 42.4% versus roughly 10–11% for every other category.
- 47 customers have not bought in over 90 days, a win-back opportunity.
- Revenue fell from about KSh 2.03M in December to 322k in January.

**Skills used:** CTEs, window functions, PL/pgSQL, views, RFM segmentation

### 🐟 [Coven Cafe Platform](https://claude.ai/artifact/7WxE6XbbTXCEU7bjhPBCVR)
A system design for a four-branch fish restaurant: point of sale, online ordering, kitchen display, per-branch inventory and a customer feedback platform, all on one central database.

**Stack:** React · Next.js · NestJS · PostgreSQL + Prisma · Socket.IO · Redis

## A taste of my SQL

Month-over-month revenue on completed orders:

```sql
WITH monthly AS (
  SELECT DATE_TRUNC('month', order_date) AS month,
         SUM(quantity * unit_price * (1 - discount / 100.0)) AS revenue
  FROM orders
  WHERE order_status = 'Completed'
  GROUP BY 1
)
SELECT month, revenue,
       revenue - LAG(revenue) OVER (ORDER BY month) AS change_vs_prev
FROM monthly
ORDER BY month;
```

## Skills

| Area | Tools and techniques |
|---|---|
| Data analysis | SQL, PostgreSQL, Excel, Power BI |
| Advanced SQL | CTEs, window functions, subqueries, PL/pgSQL, views |
| Data quality | Validation, annotation, QA, structured review |
| Growing into | Data engineering, pipelines, dashboards, cohort analysis |

## Community: Night of Code

I take part in and help organise **Night of Code**, an event where we build projects as a team, learn from one another and look out for new opportunities. It is where much of my networking and peer learning happens.

## Let's connect

Looking for a data analyst or junior data engineer? I would love to hear from you.

- 💼 LinkedIn: [calvince-okoth](https://www.linkedin.com/in/calvince-okoth-85792b25a/)
- 📧 Email: [calvinceokoth59@gmail.com](mailto:calvinceokoth59@gmail.com)
- 💬 WhatsApp: [0703 161 063](https://wa.me/254703161063)
