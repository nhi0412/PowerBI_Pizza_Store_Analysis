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

<img width="850" alt="Image" src="https://github.com/user-attachments/assets/ea0e958e-b4a8-48cd-9897-a479c4c7ae16" />

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

- Classic pizzas have the highest sales and quantity sold, followed by Supreme
- Veggie pizzas have quiet good sales but the lowest revenue => this can be the
lowest price among all categories
- Chicken, Veggie, and Supreme have quite the same quantity sold, but they greatly
differ in the revenue.

**Top & Bottom Products**

- **Top 5 by Quantity:**
    - The Big Meat Pizza
    - The Thai Chicken Pizza
    - The Five Cheese Pizza
    - The Four Cheese Pizza
    - The Classic Deluxe Pizza
- **Bottom 5 by Quantity:**
    - The Greek Pizza
    - The Green Garden Pizza
    - The Chicken Alfredo
    - The Calabrese Pizza
    - The Mexicana Pizza

Insight: Use this to focus campaigns or discontinue low performers.

**Size & Category Trends**

Chicken:

-Size L generates the most revenue (100K), followed by M (70K) and S (30K)

-No revenue from XL or XXL

Classic:

-Size L, M, and S are relatively the same (70K)

-XL and XXL have a small impact

Supreme:

-Size L generates the most revenue (90K), followed by M (70K) and S (50K)

-No revenue from XL or XXL

Veggies:

-Size L generates the most revenue (100K), followed by M (60K) and S (30K)

-No revenue from XL or XXL

### Correlation and Frequency

<img width="849" alt="Image" src="https://github.com/user-attachments/assets/2f0e5cbb-a52b-4e9e-ba89-8d92e27661b3" />

**Ingredient Sales: Correlation Between Quantity & Revenue**

- Strong positive correlation: 1.0

=> Ingredients with high quantities (buy more) tend to generate more revenue.

- 4 distinct groups:
- Top-right: High quantity and high revenue: Garlic, Tomatoes, Red Onions, Red Peppers
- Bottom-right: High quantity but lower revenue
- Top-left: Good quantity with good corresponding revenue (potential ingredients that could be promoted)
- Bottom-left: Low quantity and low revenue: large number of ingredients distributed here

**Categories Sales: Average Price vs. Quantity Correlation**

- Strong negative correlation: -0.95

=> Categories that have high prices will have low quantities sold.

- 4 distinct groups:
- Top-left: Low price and high quantity: Classic
- Bottom-left: High price and low quantity: Veggies
- Bottom-right: High price and low quantity: Supreme, Chicken

**Time Interval Between Orders**

- The peak hour is 12h, 13h, 17h, 18h, and 19h => when people have meals
- Lower orders can be seen at 14h, 15h, 20h, 21h
- It’s 23.34, the average time in minutes between orders

### Single and Multiple Item Orders

<img width="848" alt="Image" src="https://github.com/user-attachments/assets/da35caa0-c52c-4b61-9965-e304699b6bc5" />

- Multi-item orders outnumber single-item orders by ~1.5x
- Multiple-item orders (61%) are 1.5 times the single-item orders (38%) => user engagement
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
    - Consider removing or replacing bottom-tier ingredients (Brie Carre Cheese or Soppresatte Salami)
- **Campaigns Focus**
    - Marketing campaign resources focus on Quarter 2
    - Target lunch and dinner time to offer limited-time deals
