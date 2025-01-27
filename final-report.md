# E-Commerce Data Analysis Report

## Task 1: Exploratory Data Analysis and Business Insights

### Dataset Overview
- Customers: 200 unique customers across 4 regions
- Products: 100 products in 4 categories
- Transactions: 1,000 transactions from Dec 2023 to Dec 2024

### Key Business Insights

1. **Regional Performance Disparity**
   - South America leads with highest average transaction value ($721.55) and transaction count (304)
   - North America shows potential for optimization with lowest average transaction value ($624.24)
   - Europe and Asia maintain healthy mid-range performance

2. **Product Category Dynamics**
   - Books command highest average price ($292.21) with strong sales
   - Home Decor shows lowest average price ($235.02)
   - Category preferences vary significantly by region:
     * South America: Strong preference for Books
     * Asia: Leads in Clothing
     * Europe: Favors Home Decor

3. **Seasonal Transaction Patterns**
   - Peak sales occurred in July 2024 ($71,366.39)
   - Strong Q3 performance (July-September)
   - Consistent transaction volumes (94-96 transactions) during peak months

4. **Customer Purchase Behavior**
   - Remarkably consistent average items per transaction (2.43-2.60)
   - South America shows highest items per transaction (2.60)
   - North America shows lowest items per transaction (2.43)

5. **Customer Account Lifecycle**
   - Customer base spans from new (0 days) to mature accounts (1,071 days)
   - Average account age of 528 days
   - No significant correlation between account age and spending patterns

## Task 2: Lookalike Model Analysis

### Model Overview
- Implemented cosine similarity-based recommendation system
- Features used: transaction patterns, spending behavior, regional presence
- Generated top 3 recommendations for first 20 customers

### Key Findings
- High similarity scores (>0.85) achieved for most recommendations
- Strong regional clustering in recommendations
- Consistent matching of transaction patterns and spending behaviors
- Account age showed significant influence on recommendations

## Task 3: Customer Segmentation

### Clustering Results
- Optimal number of clusters: 5 (based on Davies-Bouldin Index: 1.240)
- Silhouette Score: 0.284
- Calinski-Harabasz Score: 47.455

### Cluster Profiles

1. **High-Value Mixed Region Customers (Cluster 0)**
   - Highest transactions (7.82 avg) and spend ($6,122 avg)
   - Highest average transaction value ($802)
   - Mixed regional presence (42.1% South America, 36.8% Asia)

2. **North American Standard Customers (Cluster 1)**
   - Average transactions (4.78)
   - Lower transaction value ($630)
   - Exclusively North American
   - Newer accounts (412 days average)

3. **South American Core Customers (Cluster 2)**
   - Moderate transaction count (4.42)
   - Mid-range transaction value ($641)
   - Exclusively South American
   - Mature accounts (563 days)

4. **European Premium Customers (Cluster 3)**
   - Moderate transactions (4.43)
   - Higher transaction value ($685)
   - Exclusively European
   - Established accounts (548 days)

5. **Asian Value Customers (Cluster 4)**
   - Lowest transaction count (3.63)
   - High transaction value ($689)
   - Exclusively Asian
   - Mature accounts (541 days)

### Recommendations

1. **Targeted Marketing**
   - Develop region-specific marketing campaigns
   - Focus on increasing transaction frequency in Asian market
   - Enhance value proposition in North American market

2. **Product Strategy**
   - Maintain premium pricing for Books category
   - Consider regional preferences in product placement
   - Develop cross-category promotion strategies

3. **Customer Engagement**
   - Focus on increasing transaction frequency in Cluster 4
   - Develop loyalty programs for high-value customers in Cluster 0
   - Create targeted retention strategies for newer accounts

4. **Growth Opportunities**
   - Expand high-value customer base in mixed regions
   - Focus on increasing average transaction value in North America
   - Develop strategies to move customers up-segment
