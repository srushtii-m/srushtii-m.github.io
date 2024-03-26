---
title: "Customer Segmentation Analysis"
excerpt: "This project applies K-means clustering to segment customers based on various features related to their purchasing behavior, and the analysis was focused on understanding the distinct customer groups to tailor marketing and sales strategies effectively."
collection: portfolio
---

## Data Description

The dataset includes the following features for each customer order:

- `order_item_quantity`: The number of items ordered.
- `sales`: Total sales value of the order.
- `benefit_per_order`: Profit or loss from the order.
- `order_item_discount`: Discount applied to the order items.
- `order_item_total`: Total value of the order after discount.
- `OrderDuration`: Time taken from order placement to shipping.
- `order_duration`: An alternative measure of the order processing time.

## Clustering Process

The clustering process involved the following steps:

1. **Data Preprocessing**: Data was cleaned, and features were scaled to prepare for clustering.
2. **Elbow Method**: Applied to determine the optimal number of clusters, which was found to be 4.
3. **K-Means Clustering**: The algorithm was used to segment the customer data into 4 distinct groups.
4. **Analysis**: Post-clustering analysis was performed to understand the characteristics of each cluster.

## Cluster Interpretation

The clusters were interpreted based on their centroid characteristics:

- **Segment 0**: 'Casual Shoppers' - lower in quantity and sales, less sensitive to discounts.
- **Segment 1**: 'Promotion Sensitive Buyers' - attracted by discounts, with higher sales variability.
- **Segment 2**: 'High-Spending Buyers' - characterized by high sales and order totals.
- **Segment 3**: 'Bulk Shoppers' - high quantity but moderate sales values, indicating bulk purchases.

The code and analysis is available [here](https://github.com/srushtii-m/Customer_Segmentation_Analysis)