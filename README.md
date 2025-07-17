# Amazon Product & Review Analysis (Excel Case Study)
 This case study explores Amazon product and review data using Microsoft Excel. The goal was to uncover insights that could guide product improvement, marketing decisions, and customer engagement.

# About the Dataset
 The dataset includes:
- Product names and categories
- Discounted and actual prices
- Ratings and number of reviews

# Tools Used
- Microsoft Excel
   -   Excel Tables
   -   Pivot Tables
   -   Charts (Bar,line)
   -   Formulas: IF(), COUNTIF(), basic arithmetic
   -   Formatting techniques (Number vs. Percentage)
 
# Key Metrics & Insights

1.  Product Overview
 - Number of Products by Category
 - Unique Product Count by Category
(Used Excel Table or Pivot to identify unique items per category)


2.  Pricing & Discount Analysis
 - Average Discount % by Category
```
= (Discounted Price - Actual Price) / Discounted Price
```
(Formatted as Percentage)
 - Products with 50% or More Discount
Used a helper column:
```
=IF(discount % >= 50, "Yes", "No")
```
Then applied:
```
=COUNTIF(range, "Yes")
```
- Actual vs Discount Price
Compared in a clustered bar chart

3.  Review & Engagement Metrics
- Total Review Count by Category
- Distribution of Product Ratings
- Products with < 1000 Reviews
Counted using:
```
=COUNTIF(rating_count_range, "<1000")
```
- Highest Review Count by Product
Identified top-reviewed product via Pivot Table sorting

4.  Revenue Potential
- Potential Revenue by Category
Calculated as:
```
= actual_price * rating_count
```
# Visualizations Created
The following visuals were created using Excel PivotTables and charts, all featured in the interactive dashboard:
| Visual                                         | Description                                                                                    | 
|------------------------------------------------|------------------------------------------------------------------------------------------------|
| Number of Products in Category	               | Bar chart showing the total number of products in each category. Helps identify catalog depth. |
| Price Range Bucket of Category	               | Segmented bar chart showing how products in each category fall into three price ranges: <₹200, ₹200–₹500, and >₹500. |
| Average of Actual & Discounted                 | Price by Category	Line chart comparing the average listed price and discounted price across categories — useful for visualizing pricing differences. |
| Average Discount % by Category	               |  Horizontal bar chart highlighting how much discount (on average) is applied in each product category. |
| Average Potential Revenue by Category	         |  Line chart estimating potential revenue per category using actual_price × rating_count. Shows where business value lies.|
| Average Rating Count by Category	             |  Bar chart showing the average number of reviews per category — an indicator of customer engagement and popularity. |

# Challenges & Learnings
As a beginner, I faced challenges in:
- Formatting formulas to show correct percentages (e.g., fixing 4125% to 41.25%)
- Understanding how Excel treats number formats inside PivotTables
- Using COUNTIF properly with helper columns
- Figuring out how to visually present meaningful insights
Through trial and error, I learned to:
- Use correct number formatting for calculated fields
- Create helper columns to simplify logic
- Use PivotTables for structured summaries
- Start small and build toward a complete dashboard

 # Final Excel Dashboard
The final output of this analysis is a dynamic Excel dashboard that provides clear, visual answers to business-critical questions around product variety, pricing strategy, and customer engagement.

# Dashboard Highlights
The dashboard was built using:
- Pivot Tables
- Slicers
- Helper columns
- Bar, Line, and Combo Charts
It features interactive elements for filtering by Price Range and Product Category.

# Interactivity
The dashboard includes Slicers for:
- Price Range Bucket
- Category 1

These filters allow users to dynamically view insights specific to selected ranges or categories, 
making the dashboard more interactive and user-friendly.

## Dashboard 
<img width="1891" height="809" alt="Screenshot 2025-07-17 161342" src="https://github.com/user-attachments/assets/c6e54c5b-b682-4bf0-863b-e297e9a177b4" />

## Pivot Table


<img width="1815" height="795" alt="Screenshot 2025-07-17 161503" src="https://github.com/user-attachments/assets/fa3e0835-4443-4182-9f22-888be58cbaf2" />









