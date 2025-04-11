# PowerBI_Pizza_Store_Analysis
## 1. Introduction and Motivation

The store manager wants to have real-time insights into sales performance, which is essential for running efficient operations, optimizing product availability, and increasing revenue. This Power BI dashboard was developed to give store managers a visual overview of key business metrics across all pizza categories and time periods.

With this dashboard, store managers can:

- Monitor daily, weekly, and monthly sales trends to align staffing and inventory
- Identify best-selling and low-performing pizzas by size, category, and ingredients
- Adjust in-store promotions and pricing strategies in response to sales patterns
- Launch timely campaigns during slow periods or peak days

By turning raw transaction data into actionable insights, the dashboard enables managers to make faster, smarter decisions — improving both customer satisfaction and business performance at the store level.

## **2. Introduction to Dataset**

A transactional dataset recording every pizza order placed throughout the year 2015. Each row represents an item sold and includes information such as:

- Order ID, Date, Time
- Pizza Name, Category, Size, Price
- Quantity sold and Ingredients

## **3. Business Questions**

### Sales Performance

- What are the total revenue, total orders, and average order value for 2015?
- How did daily, weekly, and monthly sales vary?
- What were the peak sales periods and seasonal patterns?
- Are there sales anomalies worth investigating?

### Product & Size Analysis

- Which pizza categories and individual pizzas performed best/worst?
- What size sells the most within each category?
- Which ingredients drive the most and least sales?

### Customer Ordering Behavior

- What’s the ratio of single-item to multi-item orders?
- What is the average time between orders?
- How do time of day and day of week influence sales?

### Pricing and Correlation Insights

- Is there a correlation between price and sales volume?
- How do quantity and revenue vary with ingredients?

## 4. Design Thinking

### **Empathize** – *Understand the stakeholder's needs*

- **Who is the stakeholder?**
    
    ➤ Store Managers
    
- **When do they use the dashboard?**
    
    ➤ Daily or weekly — before store opening, end-of-day review, or weekly planning
    
- **Why is this analysis needed?**
    
    ➤ Monitored product performance, adjusted promotions, managed stock levels, and planned staff accordingly
    
- **How do they make decisions?**
    
    ➤ Based on which pizzas sell best, what sizes are trending, when sales peak, and what underperforms
    

⇒ Problem Statement: Store managers need a way to monitor real-time sales performance, product demand, and customer buying behavior to make quick, informed decisions on inventory and promotions.

<img width="628" alt="Image" src="https://github.com/user-attachments/assets/bbd370ec-78f7-43df-8085-1acc8d6673b4" />
Empathy Map

### Define Point of View (POV) - What's the core problem

**North Star Metric**

> Daily Sales Efficiency = Revenue + Quantity Sold per Time Unit (e.g., per hour/day)
> 

This metric reflects the core value the dashboard delivers to store managers:

- It helps monitor if the store is performing efficiently based on real-time sales.
- It allows managers to adjust staffing, stock, or campaigns immediately based on actual results.

**Point of View (POV)**

- Sales by Category, Day of Week
- Time-based Sales
- Product-Level Analysis
- Order Type
- Price Impact
- Size Performance

### **Ideate – Brainstorming Dashboard Components**

- KPI Cards: Total Revenue, Orders, Quantity, AOV
- Line/Area charts: Monthly/Daily/Weekly sales trend
- Bar charts: Revenue & Quantity by Category
- Heatmap: Sales by Day & Time
- Scatter plot: Correlation between price & sales
- Table: Top 5 and Bottom 5 Pizzas
- Stacked bar chart: Pizza size breakdown

### Prototype and Review

- Can store managers **quickly see what to stock or promote**?
- Can they **respond to slow days with targeted campaigns**?
- Is the layout intuitive and mobile/desktop-friendly?

## 5. Visualization

### Overview

<img width="850" alt="Image" src="https://github.com/user-attachments/assets/9b4613b8-4f84-4e58-b357-ae7da9efc62d" />

**Sales Trends & Seasonal Patterns**

- Peak Month: July ($72.5K)
- Other Strong Months: May, November, March (~$70K)
- Low-Performance Months: September, October, December (~$64K)

Insight:

- High sales align with mid-Q1 to mid-Q3, possibly due to promotions, holidays, or school breaks.
- Q4 dip may result from budget fatigue or fewer promotions.

**Sales by Day of Week & Time**

- Top Sales Day: Friday ($136K)
- Other Strong Days: Saturday, Thursday (~$123K)
- Weakest Day: Sunday ($99K)

By Hour:

- Peak Hours: 12 PM, 1 PM, 5 PM–7 PM
- Low Hours: Midnight and post-lunch hours (2 PM–3 PM, 8 PM–9 PM)

Insight:

- Sales concentrate during lunch and dinnertime, especially on weekends.

**Category Performance**

- Best-selling Category: Classic (highest revenue & quantity)
- Veggie: Good quantity but lowest revenue → likely due to lower pricing
- Supreme & Chicken: Similar quantity but different revenue levels

**Top & Bottom Products**

- **Top 5 by Quantity:**
    - Classic Deluxe Pizza
    - Barbecue Chicken Pizza
    - Hawaiian Pizza
    - Pepperoni Pizza
    - Thai Chicken Pizza
- **Bottom 5 by Quantity:**
    - Brie Carre Pizza
    - Mediterranean Pizza
    - Calabrese Pizza
    - Spinach Supreme Pizza
    - Soppressata Pizza

Insight: Use this to focus campaigns or discontinue low performers.

**Size & Category Trends**

- Popular Sizes: S, M, L
    - Classic sells best in Size S
    - Veggie and Chicken perform well in Size L
- Underperforming Sizes: XL and XXL (minimal sales)

### Correlation and Frequency

<img width="849" alt="Image" src="https://github.com/user-attachments/assets/59ce23a6-5ca9-4f01-a7c1-1172d6a413e4" />

**Ingredient Sales: Correlation Between Quantity & Revenue**

- Correlation Coefficient: +0.93 (strong positive)
- Insight: Ingredients with high quantity sold also bring in more revenue.

Segmented Insights:

- Top-Right: High quantity + High revenue → Star ingredients
- Bottom-Right: High quantity but lower revenue → Low-margin ingredients
- Top-Left: Low quantity but high revenue → Premium potential
- Bottom-Left: Low usage and low return → Re-evaluate

**Categories Sales: Average Price vs. Quantity Correlation**

- **Correlation Coefficient:** -0.95 (strong negative)
- **Insight:** Higher-priced categories have lower sales volume

Segmented Insights:

- Top-Left: Low price, high quantity (Classic) → Popular, accessible items
- Bottom-Right: High price, low quantity (Chicken, Supreme) → Premium but low demand
- Consider repositioning or promotional pricing

**Order Frequency by Time**

- High Order Times: 12 PM, 1 PM, 5–7 PM
- Low Order Times: 2–3 PM, 8–9 PM

### Single and Multiple Item Orders

<img width="848" alt="Image" src="https://github.com/user-attachments/assets/bae43bed-5f93-402f-9af7-172c299e9a91" />

- Multi-item orders outnumber single-item orders by ~1.5x
- Insight: Customers tend to purchase more than one pizza per order, indicating potential for upselling and bundling strategies.

## 6. Business Recommendations

- **Run Bundle Promotions**
    - "Any 2 for $X", "Buy 1 Get 1 Half Off", or "Spend $Y, Save Z%"
    - Use best-selling pizzas like Classic Deluxe or Barbecue Chicken
- **Time-Based Offers**
    - Focus promotions during off-peak days (Sunday, early afternoons)
    - Launch “Weekend Combos” or “Lunch Hour Specials”
- **Upsize Incentives**
    - Encourage upsizing to M/L with “Upsize for $X” deals
- **Veggie Pizza Boost**
    - Add premium topping options to increase AOV
    - Market them as healthy or gourmet choices
- **Optimize Inventory by Size**
    - Focus inventory on S, M, and L sizes
    - Review the cost-benefit of keeping XL and XXL
- **Ingredient Strategy**
    - Highlight top-performing ingredients in product design
    - Consider removing or replacing bottom-tier ingredients
