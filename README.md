#  Vendor Performance & Inventory Analytics Dashboard

##  Project Overview

This project is a **company-level, end-to-end data analytics solution** built to analyze **vendor performance, profitability, and inventory efficiency** in a retail/wholesale business context.

The dashboard is designed to help **management, procurement, finance, and operations teams** make **data-driven decisions** related to vendor selection, pricing strategy, inventory optimization, and cost control.

The project follows a **real-world analytics workflow** using:

* **Python (Pandas, NumPy)** for data cleaning & feature engineering
* **Power BI** for interactive dashboards & business storytelling

---

##  Business Problem

Retail and wholesale businesses often work with **hundreds of vendors**, but lack clear visibility into:

* Which vendors are truly **profitable**
* Which vendors are **loss-making or inefficient**
* How inventory is being utilized across brands
* Where capital is blocked due to **slow-moving inventory**

### Key Business Risks

* Continuing contracts with loss-making vendors
* High inventory holding costs
* Poor vendor negotiations without data
* Delayed or manual reporting

---

##  Business Questions Answered


<img width="1163" height="655" alt="Screenshot 2026-01-06 090050" src="https://github.com/user-attachments/assets/cca8067f-89c5-4238-9c8a-877058215ae8" />

This dashboard answers critical management questions:

1. Who are the **top and bottom performing vendors** by profit?
2. How is **revenue distributed** across vendors?
3. Which vendors have **high revenue but low margins**?
4. How efficiently is inventory being utilized (inventory turnover)?
5. How can vendors be **segmented** for better procurement strategy?

---

##  Data Sources

The project uses multiple real-world datasets (CSV files):

| Dataset             | Description                            |
| ------------------- | -------------------------------------- |
| sales.csv           | Sales transactions and revenue details |
| purchases.csv       | Vendor purchase and cost data          |
| purchase_prices.csv | Unit purchase prices by brand          |
| begin_inventory.csv | Opening inventory levels               |
| end_inventory.csv   | Closing inventory levels               |
| vendor_invoice.csv  | Vendor invoice metadata                |

These datasets simulate **real company data spread across departments**.

---

##  Data Cleaning & Preparation (Python)

Performed in **Google Colab** using Pandas:

* Removed duplicates and handled missing values
* Standardized column names and date formats
* Merged datasets using business keys (Brand, VendorName)

### Key Derived Metrics

* **Revenue** = Sales Quantity × Sales Price
* **Cost** = Sales Quantity × Purchase Price
* **Profit** = Revenue − Cost
* **Profit Margin (%)** = Profit / Revenue × 100
* **Average Inventory** = (Begin Inventory + End Inventory) / 2
* **Inventory Turnover** = Sales Quantity / Average Inventory

---

##  Vendor Scorecard (Core Analysis)

A **vendor-level scorecard** was created to summarize performance:

* Total Sales Quantity
* Total Revenue
* Total Profit
* Average Profit Margin

### Vendor Segmentation

Vendors were segmented using **profit-based quantiles**:

* **High Performing** (Top 30%)
* **Medium Performing** (Middle 40%)
* **Low Performing** (Bottom 30%)

This segmentation supports **strategic vendor decisions**.

---

##  Power BI Dashboard Overview

The final Power BI dashboard is structured into **four professional sections**:

<img width="1163" height="655" alt="Screenshot 2026-01-06 090050" src="https://github.com/user-attachments/assets/78618f08-855f-4923-873a-22d0ab26b993" />


###  1. Executive Summary

* Total Revenue
* Total Profit
* Average Profit Margin
* Total Vendors

Provides a **quick health check** of the business.

---

###  2. Vendor Performance Analysis

* Top Vendors by Profit (Bar Chart)
* Vendor Category Distribution (Donut Chart)
* Vendor Detail Table (Revenue, Profit, Margin)

Helps identify **strategic vendors and underperformers**.

---

###  3. Profitability Insights

* **Profit % vs Revenue Scatter Plot**

  * Identifies vendors with high revenue but low margins
  * Highlights pricing and negotiation risks

---

###  4. Inventory & Operations Analysis

* Inventory Turnover by Brand
* Identification of slow-moving brands

Supports **inventory optimization and cost reduction**.

---

##  Interactivity Features

* Slicers for:

  * Vendor Category
  * Vendor Name
* Cross-filtering between charts
* Dynamic tables and visuals

These features allow **self-service analytics** for business users.

---

##  Key Business Insights

* A small group of vendors contributes **majority of total profit** (Pareto principle)
* Several vendors generate revenue but operate on **low margins**
* Inventory turnover varies significantly across brands
* Slow-moving inventory highlights opportunities to **reduce holding costs**

---

##  Business Impact

This dashboard enables:

* Data-driven vendor negotiations
* Identification of loss-making vendors
* Better inventory planning
* Faster and more confident decision-making

---

##  Tools & Technologies

* **Python** (Pandas, NumPy)
* **Google Colab**
* **Power BI Desktop**
* **CSV / Excel Data Sources**

---

##  Conclusion

This project demonstrates the ability to:

* Translate business problems into analytical questions
* Perform end-to-end data analysis
* Build professional dashboards used in real companies
* Communicate insights effectively to stakeholders

It reflects **real-world analytics skills** suitable for **internships, analyst, and entry-level data roles**.

---
