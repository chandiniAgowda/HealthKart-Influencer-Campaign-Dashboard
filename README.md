# HealthKart Influencer Campaign Dashboard

##  a. Project Overview

HealthKart runs multi-brand influencer campaigns across social media platforms to promote wellness and fitness products. To evaluate marketing effectiveness, an analytical dashboard is required.

**Objective**:  
Build an insightful dashboard to visualize influencer campaign performance, influencer ROI, engagement trends, and payout tracking using simulated datasets.


##  b. Datasets

All datasets were generated using `HealthKart_Influencer_Campaign_Notebook.ipynb`.

- **Note**: The data generation cells in the notebook are commented for safety. To regenerate, **uncomment and run** them.  
- Alternatively, **pre-generated datasets** are available and can be loaded directly into Power BI.

### Datasets Simulated:
1. `influencers.csv` — influencer profiles  
   Columns: `id`, `name`, `category`, `gender`, `follower_count`, `platform`

2. `posts.csv` — post engagement data  
   Columns: `influencer_id`, `platform`, `date`, `url`, `caption`, `reach`, `likes`, `comments`

3. `tracking_data.csv` — campaign tracking data  
   Columns: `source`, `campaign`, `influencer_id`, `user_id`, `product`, `date`, `orders`, `revenue`

4. `payouts.csv` — payment tracking  
   Columns: `influencer_id`, `basis`, `rate`, `orders`, `total_payout`


##  c. Tools Used

- **Python** (for data simulation & preprocessing)  
  Libraries: `pandas`, `numpy`, `faker`, `datetime`, `random`, `gender-guesser`

- **Power BI** (for dashboard building and analysis)



##  d. Key Performance Indicators (KPIs)

Here are some of the most important KPIs you can track to measure the success of your influencer marketing campaigns:

*   **Return on Ad Spend (ROAS)**: This measures the revenue generated for every dollar spent on advertising. It's a crucial metric for understanding the profitability of your campaigns.
    *   `ROAS = Total Revenue / Total Payout`
*   **Return on Investment (ROI)**: This is similar to ROAS but takes into account the net profit.
    *   `ROI = (Total Revenue - Total Payout) / Total Payout`
*   **Engagement Rate**: This measures how much your audience is interacting with your content. It's a good indicator of how well your content is resonating with your audience.
    *   `Engagement Rate = (Likes + Comments) / Reach`
*   **Incremental ROAS**:
    *    `Incremental ROAS = Campaign ROAS - Average ROAS Across Campaigns`


*   **Influencer Type Classification**:

    | Type      | Follower Count |
    |-----------|----------------|
    | Celebrity | ≥ 500,000      |
    | Macro     | ≥ 100,000      |
    | Mega      | ≥ 50,000       |
    | Micro     | ≥ 10,000       |
    | Nano      | < 10,000       |


##  e. Dashboard Description

A 3-page Power BI dashboard was built to offer full campaign and influencer performance visibility.

### Campaign Overview
- KPIs: Revenue, Orders, Payouts, ROAS
- Filters: Brand, Product, Platform, Influencer Type, Date Range
- Visuals: ROAS by Category, Revenue Trend, Gender Distribution

### Influencer Insights
- Top influencers by posts, followers, revenue
- Orders & ROAS by gender and category
- Follower Count vs Revenue bubble chart
- Distribution by platform and influencer type

### ROI & Payout Analysis
- Incremental ROAS by Campaign
- ROI by Category
- Best Persona & Poor ROI Influencers
- ROAS vs Total Payout by Category
- Detailed Influencer Table: ROI, ROAS, Engagement, Performance Score


##  f. Assumptions

- All data is synthetically generated based on realistic distributions.
- Engagement rate simulated between 3% to 6% based on category.
- Influencers receive payouts either per post or per order.
- Campaigns have a 6-month duration and are run across 4 platforms.
- Influencer performance is measured through a composite score of ROAS, ROI, engagement rate, and incremental ROAS.


##  g. How to Use / Reproduce

1. Open the `HealthKart_Influencer_Campaign_Notebook.ipynb` notebook.
2. Uncomment the data generation cells (clearly marked) and run the notebook.
3. Generated CSV files (`influencers.csv`, `posts.csv`, etc.) will be saved in your working directory.
4. Open Power BI → Import all CSVs → Use filters and visuals to explore insights.

> Alternatively, use the pre-generated dataset files to skip Python execution.
> Alternatively, open `HealthKart Influencer Campaign Dashboard.pbix`to see the insights created.



**Prepared by:** Chandini A  
**Internship Assignment:** HealthKart – Analytics & Data Science  
**Submission Includes:** Python Notebook, Power BI Dashboard, README File, Insights Summary (separate)
