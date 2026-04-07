# eniac_data_analysis_project: E-Commerce Sales & Discount Analysis
This project focuses on cleaning, merging, and analyzing a complex retail dataset consisting of three main components: Orders, Orderlines, and Product Catalog. The goal was to uncover how pricing strategies and seasonality drive revenue.
Key Business Questions Addressed

Product Categorization: How should products be classified to simplify reporting?
Price Distribution: What does the pricing landscape look like across different categories?
Discount Impact: How many products are discounted, and how aggressive are those price cuts?
Seasonality & Trends: How do major events like Black Friday and Christmas impact sales volume and margins?
Data Strategy: How can the current data collection process be improved for better future insights?

Data Processing Workflow
Data Merging: Combined three DataFrames using a relational structure (linking orders, orderlines, and products via sku and order_id).
Data Cleaning: * Handled missing values (NaNs) by cross-referencing unit prices and product lists.
Removed duplicate entries to ensure accurate revenue reporting.
Filtered out incomplete order states (e.g., cancelled or pending) to focus on realized revenue.
Feature Engineering: Created new calculated columns for:
Total Revenue (Quantity × Unit Price)
Discount Percentage (Difference between List Price and Paid Price)
Period Type (Flagging dates for Black Friday and Holiday seasons)

Preliminary Insights
Seasonality: Identified significant revenue spikes during the Q4 holiday window
Discount Strategy: Analyzed the correlation between high-percentage discounts and total units sold to determine if heavy discounting actually increases net profit.
Price Architecture: Visualized how different product types (e.g., accessories vs. hardware) are priced and which categories are most frequently discounted.

