# PowerBI | Global Superstore Market Expansion Strategy

## 📋 Table of Contents
1. Overview
2. Introduction to Dataset
3. Design Thinking
4. Visualizations & Key Insights
5. Recommendations

---

## 📌 Overview
### 📂 Dataset

Global Superstore Sales is a dataset containing worldwide sales records for a company called Superstore. The company operates across multiple markets spanning several continents. As the company is experiencing strong growth, it aims to increase revenue across its markets to further expand market share.

### 🎯 Project Objective

The goal of this project is to build a Power BI dashboard that enables Senior Managers to understand the company’s business performance and make data-driven decisions regarding market expansion and strategic product selection.

Senior Managers are primarily focused on three key questions:
1. What is the overall business performance?
2. How are the different markets performing?
3. How are the various product categories performing?

---

## 📕 Introduction to Dataset
The dataset consists of **three tables:**
<details>
  <summary> 📊 Table 1: Orders – Contains detailed transaction and customer information (Click to see details)</summary>

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
  <summary>📊 Table 2: People - Stores information about sales representatives in each region (Click to see details)</summary>

  <br>

  | Column Name | Data Type | Description |
  |-------------|-----------|-------------|
  | Person      | VARCHAR   | Name of the salesperson. |
  | Region      | VARCHAR   | Geographic region where the salesperson operates. |

</details>

<details>
  <summary>📊 Table 3: Returns - Stores data on returned orders (Click to see details)</summary>

  <br>

  | Column Name | Data Type | Description |
  |-------------|-----------|-------------|
  | Returned    | VARCHAR   | Indicates whether the order was returned (e.g., 'Yes' or 'No'). |
  | Order ID    | VARCHAR   | Unique identifier for each order. |

</details>

---

## 🧠 Design Thinking
### 📌 Stage 1 - Empathize
<img width="1021" height="551" alt="image" src="https://github.com/user-attachments/assets/b7b2c8d4-0098-471f-ae73-b2f87ce8d985" />
<img width="1126" height="658" alt="image" src="https://github.com/user-attachments/assets/2969d805-2b72-4d47-a86e-575b32d72250" />

### 📌 Stage 2 - Define Point of View
<img width="1200" height="609" alt="image" src="https://github.com/user-attachments/assets/7a0649bc-749e-4a0a-ab3f-380c6f413483" />

### 📌 Stage 3 - Ideate
<img width="1136" height="582" alt="image" src="https://github.com/user-attachments/assets/1b431207-d15b-46f6-a270-5e05b261db63" />

---

## 📊 Visualizations & Key Insights
### I. Overview
<img width="1600" height="897" alt="image" src="https://github.com/user-attachments/assets/8c426190-5ecb-4e5b-9c72-299d2889b24f" />

#### 🔎 Key Insights
- Business Performance: Revenue and Profit show strong growth, indicating the company is in solid expansion phase. Orders are growing in line with sales, while Profit Margin (~11.6%) remains stable → signaling sustainable growth.
- Core Markets: APAC & EU - Largest revenue base with stable margin (~12-13%). Require continued investment to maintain leadership.
- High-potential Market: Canada - Small revenue but exceptionally high profit margin (26.62%). A promising niche market with expansion potential if scale increases.
- Product: Phones and Copiers have high profit contribution with healthy demand levels, making them suitable as strategic products.

### II. Market Analysis
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/b4a785c7-0221-4bfa-b24a-944e534c0756" />

#### 🔎 Key Insights
**🛒 Market**
- APAC & EU: These are Core Markets. Largest revenue with strong YoY growth (~51–55%). High absolute profit but only average profit margin (~12–13%) →  Continue investing, focus on margin improvement (reduce discounts, optimize logistics).
- US & LATAM: These markets have high revenue but suboptimal profitability. Solid sales (~$2M) but relatively low YoY growth (US 46.9%, LATAM 48.5%). Below-average profit margin (~10–12%) → Optimize costs, improve pricing strategy and product mix to raise margins.
- Canada: This is small but highest margin market. Low revenue but outstanding profit margin (~28%) → Potential to expand and position as a premium niche market.
- Africa & EMEA: These are Weak Markets - Low sales and margins despite high YoY growth → Not a priority for major investment; maintain presence and use as test markets for new products/models.

**👩 Sales Representatives**
- Anna Andreadi is the top performer with highest total sales (~$2.8M), significantly outperforming all other reps. She could take on a leadership role in training or best practice sharing for other reps.
- Nicole Hansen is the only sales representatives in Canada, which presents both an operational risk and a growth limitation. It is advisable to retain Nicole as the lead representative for Canada and capitalize on her proven performance by involving her in onboarding and training new team members.

### III. Product Analysis
<img width="1595" height="898" alt="image" src="https://github.com/user-attachments/assets/cd3cd64e-0f00-4a59-a138-bdad73bc7bd6" />

#### 🔎 Key Insights
- Art, Storage, Binders are high-order, low-profit categories. It is suggested to position these items as entry products to attract customers, then bundle with higher-margin products (cross-sell & bundling) and use these products in promotional campaigns or loyalty initiatives to drive customer retention and upsell to profit-driving categories (marketing & loyalty programs).
- Copiers, Phones are high-profit categories. Prioritize growth in high-potential regions (e.g. Canada) to capture both new demand and superior margins.

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
