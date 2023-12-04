# Overview
This analysis is to solve a Supply Chain Issue in the FMCG domain, provided by Codebasics. 
>
Here is the [Challenge](https://codebasics.io/challenge/codebasics-resume-project-challenge/5).
>
Interactive [Dashboard](https://www.novypro.com/project/atliq-mart---supply-chain-analysis-dashboard-power-bi).
>
![image](https://github.com/thupham16/Supply-Chain-Analysis-Atliq-Mart/assets/119646834/af5e84a8-6df9-4089-bcbe-7ec0d20838b8)

# Problem and Business Requirements
## Problem
AtliQ Mart is a growing FMCG manufacturer headquartered in Gujarat, India. It is currently operational in three cities Surat, Ahmedabad and Vadodara. They want to expand to other metros/Tier 1 cities in the next 2 years.

AtliQ Mart is currently facing a problem where a few key customers did not extend their annual contracts due to service issues.
- Speculated issue: Essential products were either not delivered on time or not delivered in full over a continued period

## Business Requirement
Management wants to fix this by tracking the ‘On time’ and ‘In Full’ delivery service level for all customers daily basis.
- Metrics on daily basis and vs target, split by cities and customers
- Matrix visual for Customer and All the metric – apply conditional formatting based on gap vs target
- KPI performance vs Target over Month – drillable for weeks an days
- KPI for products in details

## Business - related term
- On time (OT %) = Number of orders delivered On Time / Total Number of Orders
- In full (IF%) = Number of Orders delivered in Full Quantity/ Total Number of Orders
- On Time in Full (OTIF %) = Number of Orders delivered both IN full & On Time/ Total Number of Orders
-	Line fill rate (LIFR%) = number of order lines shipped in Full quantity/ total order lines
-	Volume fill rate (VOFR%) = total quantity shipped/ total quantity order

# Data Modeling
This data model show the relationships between Fact Line and Fact Header with Dim tables.
>
![image](https://github.com/thupham16/Supply-Chain-Analysis-Atliq-Mart/assets/119646834/6936ecf2-bb9a-450f-a66d-7e918e2b76c7)

# Insight
- Top 6 customers account more than 50% of total number of orders: Lotus Mart, Acclaimed Stores, Vijay Stores, Rel Fresh, Coolblue and Prepel Mart.
- The dairy category is highly preferred among our customers, nearly double Food and beverages, including top popular products AM Milk 100/250/500, AM Curd 50/100/250.
- Our orders are evenly distributed among our primary markets: Ahmedabad, Surat, and Vadodara.
- Significant underperformance persisted from March to August 2022, with all KPIs consistently 20-30% below target, in which OTIF rate is the poorest performance, with a significant ~37% gap from the target, indicating weak delivery capability.
- Approximately 41% of orders experienced delayed delivery, indicating a significant portion of customers did not receive their orders within the expected timeframe. Meanwhile, 47% of the orders were delivered partially, suggesting that there may be stock shortages impacting our ability to fulfill the requested quantity.
-	On average, customers experienced a delay of approximately 0.42 days per order, indicating that each customer encountered a delay of approximately 0.42 days in receiving their orders.
-	Customers need special attention: Lotus Mart, Coolbluee and Acclaimed Stores – high demand but experience bad service with over 70% of their orders being delayed and only~50-60% their lines are fulfilled completely.
-	Product AM butter 250, AM Biscuit 250/500, AM Tea 250 often face stock shortages that lead to low LIFR rate.
-	Customers in Vadodara city are are facing the most unfavorable experience, with lowest rates across all KPIs.
-	Over the past few months, there has been no improvement across all KPIs.
# Improvement Room
-	Need to investigate the reasons for low performance
  - Low Infull Rate: 
      - Due to insufficient stock => reevaluate demand planning by aligning it with Forecast market demand to ensure adequate stock
      - Or an excessive influx of orders beyond our supply capabilities => Reassess employee capability or logistics proficiency to improve timely delivery of goods to customers.
  - Low On time Rate
      - The agreed delivery date may be overly optimistic or unrealistic.
      - Low logistics capabilities.
- In addition to enhancing our service performance, it is essential to prioritize building relationships with key customers, promptly taking action to understand their needs and ensure their satisfaction.
# Key Learning
- Gaining  domain knowledge and business terms in Supply Chain domain.
- Designing dashboards and utilizing diverse visual elements to meet specific user requirements.
- Usage of buttons to navigate to different visuals via bookmarks.
- Writing complex DAX measures for visualization and conditional formatting.
