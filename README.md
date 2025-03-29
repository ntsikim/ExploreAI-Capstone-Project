# Telecom Customer Segmentation & Insights Using K-Means Clustering

A Data-Driven Exploration of Customer Behavior and Business Opportunities

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Objective & Motivation](#objective--motivation)  
3. [Dataset Description](#dataset-description)  
4. [Data Preprocessing](#data-preprocessing)  
5. [Feature Engineering](#feature-engineering)  
6. [Clustering with K-Means](#clustering-with-k-means)  
7. [Insights & Business Implications](#insights--business-implications)  
8. [Power BI Dashboard](#power-bi-dashboard)  
9. [Conclusion & Next Steps](#conclusion--next-steps)  
10. [Deliverables](#deliverables)  
11. [Usage](#usage)  
12. [Acknowledgements](#acknowledgements)  
13. [Author](#author)

---

## Project Overview

This project applies K-Means Clustering to segment telecom customers into meaningful groups based on usage behavior, subscription types, and demographic factors. The insights empower marketing, customer retention, and operational teams to target customers more effectively.

---

## Objective & Motivation

### Objective:
To segment telecom customers into distinct clusters using K-Means Clustering for personalized marketing, churn reduction, and product optimization.

### Motivation:
- High churn rates and diverse customer behavior challenge the telecom industry.
- Traditional segmentation misses important behavioral signals.
- Unsupervised learning helps reveal hidden customer patterns and growth opportunities.

---

## Dataset Description

- Source: Anonymized dataset sourced from Kaggle
- Size: ~7,000 customer records
- Features:
  - Demographic: Age, Dependents, Zip Code, Location
  - Usage: GB download, Long Distance Charges, Tenure
  - Services: Internet, Streaming, Tech Support
  - Finance: Monthly Charges, Refunds, Payment Method
  - Customer Status: Stayed, Churned, Joined

---

## Data Preprocessing

- Removed redundant or irrelevant columns
- Encoded categorical features using Label Encoding and One-Hot Encoding
- Identified and handled missing values:
  - Avg Monthly GB Download: Imputed as 0 for customers with no internet service
  - Service-related columns (e.g., Streaming TV, Tech Support): Imputed with "No Internet"
- Normalized numerical features for clustering

---

## Feature Engineering

- Carefully selected numerical features with direct customer behavioral impact:
  - Monthly Charge, Total Charges, Tenure, Long Distance Charges, etc.
- Feature selection focused on:
  - Removing bias from categorical behavior like contract types
  - Avoiding artificial clustering based on non-behavioral traits
- Used scaling where required (e.g., revenue-based features)

---

## Clustering with K-Means

- Applied K-Means Clustering on selected numerical features
- Used the Elbow Method and Silhouette Score to identify optimal k = 5
- Each customer assigned a cluster label from 0 to 4
- Clusters interpreted using Power BI visualizations

---

## Insights & Business Implications

Key customer segments identified:

- Cluster 0: Budget-conscious, high churn, short tenure, prefer debit orders  
- Cluster 1: Internet-light, moderate churn, some streaming services  
- Cluster 2: High-value, loyal customers with long tenure and high charges  
- Cluster 3: Mid-value customers with large extra data charges  
- Cluster 4: High refund claims and risk signals despite moderate usage  

### Business implications:
- Tailored campaigns can be built per cluster  
- Churn-prone groups identified for retention targeting  
- High-value clusters provide upselling and loyalty opportunities  

---

## Power BI Dashboard

An interactive Power BI dashboard was created with visuals covering:

- Cluster size distribution  
- Total and Monthly Charges  
- Tenure, Internet Usage, Referrals  
- Revenue and Refunds  
- Customer Status (Churned, Joined, Stayed)  
- Service Adoption by Cluster  
- Geographic clustering using Latitude/Longitude  

Visuals are grouped logically in the dashboard to allow drill-down insights and storytelling.

---

## Conclusion & Next Steps

- K-Means successfully revealed 5 meaningful customer segments  
- Clear behavioral and financial patterns emerged from the clusters  
- Power BI dashboards enhanced interpretability and business understanding  

### Next Steps:
- Convert insights into marketing strategies  
- Deploy clustering pipeline to production environment  
- Explore deeper churn prediction using supervised learning  

---

## Deliverables

- README.md – Full project documentation  
- Customer_Segmentation_Clustering_Notebook.ipynb – Jupyter notebook with end-to-end analysis  
- requirements.txt – Python dependencies  
- Power BI Dashboard screenshots (embedded in presentation/report)  
- Recorded video presentation (as required by ExploreAI)  
- capstone_presentation.pptx – Presentation slides used for storytelling  

---

## Usage

To run the project locally:

### 1. Clone the repository:
- https://github.com/ntsikim/ExploreAI-Capstone-Project.git
- cd telecom-customer-segmentation
### 2. Set up virtual environment (optional but recommended):
- python -m venv venv
- source venv/bin/activate  # or venv\Scripts\activate on Windows
### 3. Install dependencies:
- pip install -r requirements.txt
### 4. Launch Jupyter Notebook:
- jupyter notebook

--- 
---

## Acknowledgements

- ExploreAI Academy – for guidance, curriculum, and support  
- Kaggle – for providing the anonymized telecom dataset  
- Power BI – for enabling powerful visual storytelling  

---

## Author

**Ntsikelelo Myesi**  
Capstone Project – 31 March 2025  
ExploreAI Academy  
GitHub: *[https://github.com/ntsikim/ExploreAI-Capstone-Project]*

