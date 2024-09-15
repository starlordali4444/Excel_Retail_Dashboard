# Dynamic Retail Dashboard in Excel

## Objective

The goal of this project is to build a **Dynamic Retail Dashboard** in Excel that provides a comprehensive analysis of sales, profit, and customer data across multiple dimensions like product categories, regions, and customer segments. This dashboard helps answer key business questions such as total sales, top and bottom-performing products, customer insights, and return analysis, offering actionable insights for data-driven decision-making.

### Key Questions Answered:
1. **KPIs**: Total Sales, Total Profit, Quantity Sold, Number of Orders, and Profit Margin.
2. **Sales and Profit Analysis**: Analyze sales and profitability trends across different categories and regions.
3. **Category-wise Profit**: Evaluate which product categories contribute the most to profit.
4. **Segment-wise Sales Share %**: Measure sales share across different customer segments (Consumer, Corporate, Home Office).
5. **Sales by Country**: Break down sales performance by country.
6. **Top 5 Subcategories**: Identify the top-performing product subcategories.
7. **Bottom 5 Subcategories**: Analyze the least-performing subcategories.
8. **Yearly Sales Trend**: Understand how sales evolve year-over-year.
9. **Return Analysis**: Examine which orders were returned and their impact on profitability.
10. **Top and Bottom Customers**: Highlight the highest and lowest revenue-generating customers.

## Data Sources

The dashboard is built using three data tables:
1. **Orders Table**: Contains data on order details including customer info, product, sales, profit, and shipping details.
2. **People Table**: Lists sales representatives by region.
3. **Returns Table**: Contains return data, indicating which orders were returned across markets.

### Sample of Orders Data:
| Order ID       | Order Date | Ship Mode    | Customer Name    | Segment   | Country        | Product Name                                    | Sales  | Quantity | Profit   | Shipping Cost | Order Priority |
|----------------|------------|--------------|------------------|-----------|----------------|------------------------------------------------|--------|----------|----------|---------------|----------------|
| CA-2012-124891 | 31-07-2020 | Same Day     | Rick Hansen       | Consumer  | United States  | Plantronics CS510 - Over-the-Head Wireless HS   | 2309.65| 7        | 762.18   | 933.57        | Critical       |
| IN-2013-77878  | 05-02-2021 | Second Class | Justin Ritter     | Corporate | Australia      | Novimex Executive Leather Armchair, Black       | 3709.39| 9        | -288.77  | 923.63        | Critical       |

### Sample of Returns Data:
| Returned | Order ID        | Market     |
|----------|-----------------|------------|
| Yes      | MX-2013-168137   | LATAM      |
| Yes      | CA-2013-118311   | United States |

---

## Steps

1. **Data Import and Cleaning**:
   - Imported data using the **Get Data** option in Excel.
   - Used **Power Query Editor** to clean the data, ensuring that each table is properly structured and formatted for analysis.
   
2. **Data Preparation**:
   - Loaded three tables: Orders, People, and Returns.
   - Joined the tables based on relevant keys like **Order ID** and **Region**.

3. **KPI Creation**:
   - Built key performance indicators (KPIs) like **Total Sales, Profit, Quantity, Average Discount, and Order Count** using Excel formulas and PivotTables.
   
4. **Dynamic Dashboard**:
   - Created multiple dynamic charts to visualize key metrics.
   - Added slicers for easy filtering by **Category, Segment, Order Priority**, etc.
   - Integrated all KPIs into a single chart for holistic performance tracking.

5. **Visuals**:
   - Used different types of charts (Bar, Line, Pie, and Table) to visualize:
     - Sales and profit trends.
     - Top and bottom-performing subcategories.
     - Segment-wise sales share.
     - Yearly sales trend.
     - Country-specific sales distribution.

6. **Return Analysis**:
   - Incorporated a table to analyze the **Order Returns** by **Market** to understand which regions face the most returns.

7. **Top and Bottom Customer Identification**:
   - Calculated and displayed the **Top Customer** by total sales and the **Bottom Customer** with the least contribution to sales.

8. **Added a Table for All KPIs in One View**:
   - Added a new table to display all major KPIs such as **Total Sales, Profit, Quantity**, etc., in a single view for easy comparison across different time periods or dimensions.

### KPI Table Sample:
| Name         | Metric             | Symbol |
|--------------|--------------------|--------|
| Total Sales  | Sum of Sales        | 🔍    |
| Total Profit | Sum of Profit       | 💰    |
| Total Quantity | Sum of Quantity   | 📦    |
| Avg Discount | Average of Discount | 💹    |
| Total Order  | Count of Order ID   | 🛒    |
| Profitability | Sum of Profit Margin | 📈  |

---

## Conclusion

The **Dynamic Retail Dashboard** provides a comprehensive view of the business's retail performance, allowing users to easily track **sales**, **profit**, **customer insights**, and **returns** in real-time. By leveraging Excel’s powerful data analysis features like **PivotTables**, **Power Query**, and **Slicers**, this dashboard enables stakeholders to make informed business decisions based on actionable insights.

Key takeaways:
- The dashboard effectively highlights both top-performing products and areas needing improvement (e.g., returns, unprofitable categories).
- It allows for quick insights into different market performances, empowering decision-makers to fine-tune strategies based on customer segments, regions, and product categories.
- It provides transparency into discount strategies and their impact on profitability.

---

## Significance

This dashboard is highly significant for:
- **Business Analysts**: Provides a clear snapshot of critical metrics like sales, profit, and customer behavior.
- **Sales Teams**: Identifies top and bottom customers, helping focus on key accounts.
- **Operations Teams**: Assesses shipping modes and order priorities to streamline logistics.
- **Strategic Decision Makers**: Empowers data-driven strategies by delivering comprehensive insights into business performance across global markets.
  
By answering critical business questions, this dashboard acts as a one-stop tool for understanding retail performance and driving growth.

---

## How to Use:

1. **Clone or Download** this repository.
2. Open the **Excel file** and explore the pre-built dashboard.
3. Use slicers to filter data dynamically across different dimensions like **category, region, segment**, and more.
4. Explore charts to get insights on KPIs, category-wise performance, customer behavior, and sales trends.
