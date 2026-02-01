# Analyze Market Expansion Opportunities For A Retail Company Using Power BI

<img width="2240" height="1260" alt="market expansion strategy" src="https://github.com/user-attachments/assets/8745d3e4-3721-49ab-a0af-673a6378c211" />

This project developes a strategic **Power BI dashboard** enabling leadership to assess the company’s overall business performance, identify market expansion opportunities, and determine priority product lines for investment.
- **Author**: Le Dang Kim Ngan
- **Tool Used**: PowerBI (PowerQuery, Data Modeling, DAX, Visualization)

---

## 📋 Table of Contents
1. Overview
2. Introduction to Dataset
3. Design Thinking Process
4. Visualizations & Key Insights
5. Recommendations

---

## ✨ Overview
Global Superstore Sales is a dataset containing worldwide sales records for a company called Superstore. The company operates across multiple markets spanning several continents. As the company is experiencing strong growth, it aims to increase revenue across its markets to further expand market share.

### 🎯 Project Objective

The goal of this project is to build a Power BI dashboard that enables Senior Managers to understand the company’s business performance and make data-driven decisions regarding market expansion and strategic product selection.

Senior Managers are primarily focused on three key questions:
1. What is the overall business performance?
2. How are the different markets performing?
3. How are the various product categories performing?

---

## 📂 Introduction to Dataset
The dataset consists of **three tables:**
<details>
  <summary> Table 1: Orders – Contains detailed transaction and customer information (Click to see details)</summary>

  <br>

  | Column Name   | Data Type | Description |
  |---------------|-----------|-------------|
  | Order ID      | VARCHAR   | Unique identifier for each order. |
  | Order Date    | DATE      | Date when the order was placed. |
  | Ship Date     | DATE      | Date when the order was shipped. |
  | Ship Mode     | VARCHAR   | Shipping method used for delivery. |
  | Customer ID   | VARCHAR   | Unique identifier for each customer. |
  | Customer Name | VARCHAR   | Full name of the customer. |
  | Segment       | VARCHAR   | Customer segment (e.g., Consumer, Corporate). |
  | City          | VARCHAR   | City where the order was placed. |
  | State         | VARCHAR   | State where the order was placed. |
  | Country       | VARCHAR   | Country where the order was placed. |
  | Postal Code   | VARCHAR   | Postal code of the shipping address. |
  | Market        | VARCHAR   | Market region (e.g., APAC, EMEA). |
  | Region        | VARCHAR   | Geographical region of the order. |
  | Product ID    | VARCHAR   | Unique identifier for each product. |
  | Category      | VARCHAR   | Product category (e.g., Furniture, Office Supplies). |
  | Sub-Category  | VARCHAR   | Sub-category of the product. |
  | Product Name  | VARCHAR   | Name of the product ordered. |
  | Sales         | DECIMAL   | Revenue generated from the order. |
  | Quantity      | INT       | Number of items ordered. |
  | Profit        | DECIMAL   | Profit earned from the order. |

</details>

<details>
  <summary> Table 2: People - Stores information about sales representatives in each region (Click to see details)</summary>

  <br>

  | Column Name | Data Type | Description |
  |-------------|-----------|-------------|
  | Person      | VARCHAR   | Name of the salesperson. |
  | Region      | VARCHAR   | Geographic region where the salesperson operates. |

</details>

<details>
  <summary> Table 3: Returns - Stores data on returned orders (Click to see details)</summary>

  <br>

  | Column Name | Data Type | Description |
  |-------------|-----------|-------------|
  | Returned    | VARCHAR   | Indicates whether the order was returned (e.g., 'Yes' or 'No'). |
  | Order ID    | VARCHAR   | Unique identifier for each order. |

</details>

**Data Relationships:**

This project uses a **star-schema** model. The **Orders** table serves as the central **fact table**, connected to multiple dimension and supporting tables through **one-to-many** relationships.

<img width="1022" height="706" alt="image" src="https://github.com/user-attachments/assets/b58c5899-e785-4d77-ad91-a75adf8583d0" />

---

## 🧠 Design Thinking Process
### 📌 Stage 1 - Empathize
<img width="1021" height="551" alt="image" src="https://github.com/user-attachments/assets/b7b2c8d4-0098-471f-ae73-b2f87ce8d985" />
<img width="1126" height="658" alt="image" src="https://github.com/user-attachments/assets/2969d805-2b72-4d47-a86e-575b32d72250" />

### 📌 Stage 2 - Define Point of View
<img width="1199" height="607" alt="image" src="https://github.com/user-attachments/assets/4d9b6f4e-ae58-4c4a-aed3-807c9f72457b" />

### 📌 Stage 3 - Ideate
<img width="1138" height="584" alt="image" src="https://github.com/user-attachments/assets/9ef8fa94-c1b5-401d-a334-69ada3cf6b45" />

---

## 📊 Visualizations & Key Insights
### I. Overview
<img width="1440" height="808" alt="image" src="https://github.com/user-attachments/assets/f9b3ab2b-1b14-48cc-8b51-7cbcdc83dbbe" />

#### 🔎 Key Insights
- Business Performance: Revenue and Profit show strong growth, indicating the company is in solid expansion phase. Orders are growing in line with sales, while Profit Margin (~11.6%) remains stable → signaling sustainable growth.
- Core Markets: APAC & EU - Largest revenue base with stable margin (~12-13%). Require continued investment to maintain leadership.
- High-potential Market: Canada - Small revenue but exceptionally high profit margin (26.62%). A promising niche market with expansion potential if scale increases.

### II. Market Analysis
<img width="1439" height="809" alt="image" src="https://github.com/user-attachments/assets/48f275f4-6836-4d12-9ec7-dbbdb8fd4dbb" />

#### 🔎 Key Insights
**Market**
- APAC & EU: These are Core Markets. Largest revenue with strong YoY growth (~51–55%). High absolute profit but only average profit margin (~12–13%) → Continue investing, focus on margin improvement (reduce discounts, optimize logistics).
- US & LATAM: These markets have high revenue but suboptimal profitability. Solid sales (~$2M) but relatively low YoY growth (US 46.9%, LATAM 48.5%). Below-average profit margin (~10–12%) → Optimize costs, improve pricing strategy and product mix to raise margins.
- Canada: This is small but highest margin market. Low revenue but outstanding profit margin (~28%) → Potential to expand and position as a premium niche market.
- Africa & EMEA: These are Weak Markets - Low sales and margins despite high YoY growth → Not a priority for major investment; maintain presence and use as test markets for new products/models.

**Sales Representatives**
- Anna Andreadi is the top performer with highest total sales (~$2.8M), significantly outperforming all other reps. She could take on a leadership role in training or best practice sharing for other reps.
- Nicole Hansen is the only sales representatives in Canada, which presents both an operational risk and a growth limitation. It is advisable to retain Nicole as the lead representative for Canada and capitalize on her proven performance by involving her in onboarding and training new team members.

### III. Product Analysis
<img width="1441" height="809" alt="image" src="https://github.com/user-attachments/assets/f9255fe5-3212-4a52-86b6-d09763efa096" />

#### 🔎 Key Insights
- Art, Storage, Binders are high-order, low-profit categories. It is suggested to position these items as entry products to attract customers, then bundle with higher-margin products (cross-sell & bundling) and use these products in promotional campaigns or loyalty initiatives to drive customer retention and upsell to profit-driving categories (marketing & loyalty programs).
- Tables is the weakest performer in the portfolio. It records the lowest total number of orders among all sub-categories while also generating negative total profit. This indicates both low market demand and structural profitability issues, where each additional order further erodes overall profit. Consider phasing out Tables from the strategic product portfolio and reallocating resources to higher-performing categories.
- Phones and Copiers have high profit contribution with healthy demand levels, making them suitable as strategic products. Prioritize growth in high-potential regions (e.g. Canada) to capture both new demand and superior margins.

---

## 🚀 Recommendations
| Strategy | Recommendation |
|---------|----------------|
| APAC & EU – Core engines that need efficiency tuning | Standardize discount rules to avoid unnecessary price cuts. Re-optimize logistics (warehouse consolidation, seasonal route review). Run price A/B tests by segment to find profit-optimal price points. |
| US & LATAM – If prices can’t go up, costs must go down | Audit logistics cost per product category and remove inefficient routes. Shift product mix toward Phones/Copiers and reduce reliance on Art/Storage. Use profit-led promotions instead of volume-led ones. |
| Canada – A small but golden mine | Increase targeted marketing for high-margin products. Expand sales team to reduce dependency on one rep. Build premium market positioning with fewer discounts and stronger after-sales service. |
| Africa & EMEA – Keep presence light | Maintain low-cost distribution channels only. Use these markets as testing environments for new products or pricing models. |
| Turn Anna Andreadi into the team’s force multiplier | Document her techniques into an “Anna Playbook.” Assign her as mentor for new or underperforming sales reps. |
| Reduce single-rep risk in Canada | Hire an additional rep to support the region. Have Nicole handle onboarding and training to replicate her approach. |
| Low-profit, high-volume products (Art, Storage, Binders) | Use as entry-level offerings with attractive pricing. Bundle with high-margin items like Phones/Copiers. Integrate into loyalty programs to nudge upselling. |
| High-profit products (Copiers & Phones) | Increase focus in Canada to leverage high margins. Target small and medium businesses for stable demand. Improve inventory planning in APAC/EU to lower storage costs and shorten delivery time. |
| Operations & Pricing | Implement customer-level margin tracking. Negotiate supplier terms for Phones/Copiers to boost margins by 1–2%. Apply tiered pricing in APAC/EU based on purchase volume. |
