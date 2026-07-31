# rfm-analysis-online-retail
End-to-end Customer Segmentation Analysis (RFM) and Revenue Intelligence using Excel with Power Query, and Tableau Public.

**Business Problem and Objectives**
Problem:
Marketing budget is spread equally across all customers due to lack of visibility into customer lifetime value and churn risk.
Objective:
Segment customer base using RFM modeling to optimize marketing expenditure, protect core revenue, and reduce churn.

**Key Questions:**
1. Who are our most loyal and highest-contributing customers?
2. Which customer segments are at risk of churning, and what is the monetary exposure?
3. How are revenue and customer counts distributed across RFM tiers?
4. What targeted, segment-specific strategies should be deployed?

**Key Data Insights and Takeaways**
Champions and Loyal:
Customer Count: ~2,482
Revenue Share: 79.91%
Context: Core financial driver (80/20 rule). Requires high-priority VIP retention.

At-Risk:
Customer Count: 600
Revenue Share: 4.68% (0.80M USD)
Context: Inactive for more than 400 days. Immediate automated win-back required.

New Customers:
Customer Count: 353
Revenue Share: Growth Core
Context: High initial engagement with average recency of 32 days. Prime target for second-purchase conversion.

**Data Pipeline and Methodology**
1. Data Cleaning and Inspection:
Reduced record volume from 1,067,371 to 779,425 clean records by filtering missing Customer IDs, duplicates, invalid negative values, and cancellations. Handled extreme outliers (reduced quantity variance by 48%) while preserving valid wholesale transactions. Standardized country labels into unified categories.

2. Exploratory Data Analysis (EDA):
Generated descriptive statistics and PivotTables to analyze purchasing frequency, distribution, and Average Order Value (AOV of 463.48 USD).

3. RFM Modeling and Scoring:
Calculated Recency, Frequency, and Monetary metrics per customer. Applied a Quartile-based scoring method (1-5) to define data-driven segment boundaries, grouping users into 6 distinct segments.

4. Visualization:
Designed an interactive executive dashboard on Tableau Public.

Strategic Business Recommendations
Champions and Loyal (Protect Core Revenue):
Launch an exclusive VIP Royalty Program with early access to new products rather than heavy discounts. Focus on maintaining high retention and cross-selling related inventory to boost AOV.

At-Risk Segment (Mitigate 0.80M USD Churn Exposure):
Deploy automated, time-sensitive win-back email campaigns with personalized discounts based on historical purchasing habits.

New Customers (Maximize Onboarding Value):
Implement a 30-day post-purchase onboarding sequence to drive the second transaction before engagement drops.

Lost or Low-Value Base (Budget Optimization):
Stop paid retargeting campaigns for long-inactive cohorts (>640 days recency) to maximize Return on Ad Spend (ROAS).

**Project Resources and Links**

Visualization : [View Tableau Dashboard](https://public.tableau.com/views/CustomerSegmentationRevenueIntelligenceDashboardRFMAnalyticsApproach/DashboardRFM?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
