# Dynamic-Retail-Dashboard
### Dynamic Retail Dashboard in Excel

#### Overview:
The Dynamic Retail Dashboard is a powerful tool built in Excel, designed to visualize and analyze retail data. It connects to datasets hosted on GitHub, uses Power Query for transforming the data, and presents the insights through dynamic charts and KPIs. This dashboard helps solve essential business questions, enabling effective decision-making.

#### Datasets Used:
1. **Orders Table:**
   - Contains customer order details, such as product, shipping, and financial metrics.
   
   **Sample Data:**
   | Order ID         | Returned | Order Date | Ship Date | Ship Mode  | Customer Name | Segment   | Country      | Market | Sales  | Profit  | Discount |
   |------------------|----------|------------|-----------|------------|---------------|-----------|--------------|--------|--------|---------|----------|
   | CA-2012-124891   | No       | 31-07-2020 | 31-07-2020| Same Day  | Rick Hansen   | Consumer  | United States| US     | 2309.65| 762.18  | 0        |
   | IN-2013-77878    | Yes      | 05-02-2021 | 07-02-2021| Second Class| Justin Ritter | Corporate | Australia    | APAC   | 3709.40| -288.77 | 0.1      |
   | IN-2013-71249    | No       | 17-10-2021 | 18-10-2021| First Class| Craig Reiter  | Consumer  | Australia    | APAC   | 5175.17| 919.97  | 0.1      |

2. **Returns Table:**
   - Tracks details about returned orders and their respective markets.
   
   **Sample Data:**
   | Returned | Order ID         | Market |
   |----------|------------------|--------|
   | Yes      | MX-2013-168137   | LATAM  |
   | Yes      | US-2011-165316   | LATAM  |
   | Yes      | ES-2013-1525878  | EU     |
   | Yes      | CA-2013-118311   | United States |

3. **People Table:**
   - Contains information about sales representatives and the regions they cover.
   
   **Sample Data:**
   | Person            | Region   |
   |-------------------|----------|
   | Anna Andreadi     | Central  |
   | Chuck Magee       | South    |
   | Kelly Williams    | East     |
   | Matt Collister    | West     |
   | Deborah Brumfield | Africa   |

#### Key Problems Solved:

1. **Key Performance Indicators (KPIs):**
   - Objective: Display key metrics like Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.
   
   **Steps:**
   - Import the Orders table using Power Query.
   - Create calculated columns (e.g., Profit Margin = Profit / Sales).
   - Use Excel formulas to calculate Total Sales, Total Profit, Total Quantity, etc.
   - Design a dynamic KPI table with visual symbols (e.g., 💰 for Total Sales).

2. **Sales and Profit Analysis:**
   - Objective: Identify sales and profit trends over time.
   
   **Steps:**
   - Create a Pivot Table grouped by Order Date (Year and Month).
   - Add Sales and Profit as values.
   - Use a Line Chart to visualize the trends.
   - Add slicers for dynamic filtering (e.g., by category, market, or region).

3. **Category-Wise Profit:**
   - Objective: Evaluate profitability by product category.
   
   **Steps:**
   - Create a Pivot Table with Category as rows and Profit as values.
   - Sort by Profit in descending order.
   - Create a Bar Chart to visualize the profit by category.
   - Add slicers for interactivity.

4. **Segment-Wise Sales Share:**
   - Objective: Visualize the sales share for each customer segment.
   
   **Steps:**
   - Create a Pivot Table with Segment as rows and Sales as values.
   - Calculate percentage share using the formula: `Sales / Total Sales * 100`.
   - Create a Pie or Donut Chart to represent the sales share.

5. **Sales by Country:**
   - Objective: Compare sales performance by country.
   
   **Steps:**
   - Create a Pivot Table with Country as rows and Sales as values.
   - Sort by Sales in descending order.
   - Use a Heatmap or Geographic Map Chart to highlight high-performing countries.

6. **Top 5 Subcategories:**
   - Objective: Identify the top-performing subcategories.
   
   **Steps:**
   - Create a Pivot Table with Sub-Category as rows and Sales as values.
   - Sort by Sales in descending order and filter to show the top 5.
   - Use a Column Chart to display the results.

7. **Bottom 5 Subcategories:**
   - Objective: Highlight underperforming subcategories.
   
   **Steps:**
   - Use the same Pivot Table but sort in ascending order of Sales.
   - Filter to show the bottom 5 subcategories.
   - Use contrasting colors in a Column Chart to emphasize low performers.

8. **Yearly Sales Trends:**
   - Objective: Analyze sales performance across different years.
   
   **Steps:**
   - Create a Pivot Table grouped by Year with Sales as values.
   - Use a Line Chart to visualize the trend over time.
   - Use slicers for filtering by category, region, or segment.

#### Dynamic Features:
The dashboard is designed with the following dynamic elements:

- **Dynamic Charts:** The charts update in real-time based on slicer inputs, providing an interactive experience.
- **Power Query Integration:** Data cleaning and transformation are automated with Power Query for seamless updates.
- **KPI Table:** A central table dynamically highlights critical business metrics, allowing quick insights at a glance.

#### Next Steps for Extension:
- **Return Analysis:** Investigate return rates by market or product category.
- **Top and Bottom Customers:** Identify the most and least profitable customers.
- **Market Analysis:** Compare performance across different markets.
- **Product Analysis:** Evaluate how individual products contribute to sales and profit.

#### Significance:
This dynamic retail dashboard is a valuable tool for retail businesses. It enables decision-makers to:

- Track essential KPIs.
- Understand trends in categories, segments, and regions.
- Make data-driven decisions to optimize business performance.

#### Visuals:
The dashboard comes with visual examples for each analysis, including charts, KPI tables, and slicers to enhance the overall user experience.
