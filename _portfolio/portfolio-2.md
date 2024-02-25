---
title: "Amazon Product Co-Purchasing Network Analysis"
excerpt: "This project leverages network analysis and machine learning to analyze over half a million Amazon product metadata, focusing on understanding product relationships, predicting sales ranks, and provide product recommendations"
collection: portfolio
---

### How Can We Accurately Recommend Products Based on on Amazon Using Network Analysis?

 In this project, I developed a network analysis system to analyze and recommend Amazon products, using a dataset with over half a million reviews and metadata. This involved applying network analysis, particularly centrality metrics, and regression models to predict product sales ranks. Ego graph-based methods were also used for product recommendations based on user behavior. Despite computational limitations restricting the full implementation of community detection concepts, this project offered significant insights into customer purchasing patterns and product strategies in the Amazon marketplace. The complete code is available [here](https://github.com/srushtii-m/Amazon-product-co-purchasing-network-analysis/blob/main/README.md).

![image1](/images/amazon_network.png)

### Key Components of this Project
* [Amazon Co-Purchase Network Analysis](https://github.com/srushtii-m/Amazon-product-co-purchasing-network-analysis/tree/1b1c0533d2989fe47f43e3684965f41426e173d6/Network%20Analysis)

    * Data Preprocessing: Amazon product data was structured into a dictionary, extracting key attributes such as product ID, title, category, sales rank, and reviews. The data underwent thorough cleaning and formatting, including text processing using NLTK library.
    * Network Analysis and Regression Modeling: Created a network of products based on similarities, using the Jaccard index for edge weights. Degree centrality and clustering coefficient metrics were analyzed, informing the regression model used to predict product sales ranks.
    * Community Detection Limitations: While community detection was considered for improving model accuracy, computational limitations hindered the implementation of algorithms like the Girvan Newman Algorithm.The extensive time complexity of these algorithms, relative to the size of the network, made their application impractical for this dataset.

* [Analysis of Network Centrality Metrics](https://github.com/srushtii-m/Amazon-product-co-purchasing-network-analysis/tree/1b1c0533d2989fe47f43e3684965f41426e173d6/Centrality%20Metrics)

    * Centrality Metrics Analysis in DVD Subgroup: The project focuses on analyzing the centrality metrics of the DVD subgroup (19,828 products) within Amazon's co-purchasing network, due to the full network's large size (548,552 products). Key metrics include Degree, Betweenness, Closeness, and Eigenvector Centrality, aiming to identify influential DVDs based on their network position and connections.
    
    * Identifying Influential Products: The analysis used these metrics to pinpoint the most popular DVDs (Degree Centrality), products frequently bought with others (Betweenness Centrality), and the most co-purchased items (Closeness Centrality). DVDs were also categorized by genres to further refine the analysis.

* [Product Recommendation](https://github.com/srushtii-m/Amazon-product-co-purchasing-network-analysis/tree/1b1c0533d2989fe47f43e3684965f41426e173d6/Product%20Recommendation)

    * Filtering Similar Products: For each purchased product, an ego graph is created, and products similar to the purchased item are filtered using a similarity threshold. This process narrows down the product selection to a more relevant and focused group, based on their interconnectedness in the purchasing network.

    * Ranking and Displaying Recommendations: The filtered similar products are ranked according to their average rating and total reviews. The top 5 products from this ranking are then selected, and their details like title, sales rank, and ratings are displayed to the customer as the most relevant recommendations.

