# Consumer Purchase Pattern Identification and Data Mining in Python

**Prepared by Aurel Sahiti**

---

## Executive Summary:  
In today’s retail and e-commerce landscape, understanding customer purchase patterns and the relationships between products is transformational.  
Using **Python**, this project explores transaction data to uncover buying behavior, frequent item sets, and association rules. This transforms raw purchase data into actionable insights for cross-selling, product bundling, and marketing strategy.

#### Key outcomes from the analysis include:
- Identification of high-frequency product combinations and strong association rules.  
- Discovery of distinct customer segments based on purchase behavior and recency/frequency/monetary (RFM) scores.  
- Recommendations for targeted promotions, optimized product placement, and strategic bundling.

These findings provide a framework for increasing average transaction value, enhancing customer retention, and driving incremental revenue through data-driven merchandising and marketing.

---

## Business Problem:  
Retailers often have large volumes of transaction data but lack clarity on **which products are frequently purchased together**, **which customer behaviors signal high value**, and **how to structure offers based on these insights**. Key questions addressed include:

- Which product combinations occur frequently and should be promoted together?  
- How can we segment customers based on purchase frequency, recency, and monetary value to identify high-value groups?  
- What association rules exist that can inform cross-sell, upsell, or bundle strategy?

The goal of this project was to build a **data mining workflow** in Python that identifies these patterns, segments customers, and delivers strategic recommendations from transaction data.

---

## Methodology:  
This project followed a structured analytical workflow using Python for data mining:

1. **Data Ingestion & Preparation**  
   - Imported transaction data from CSV files.  
   - Cleaned and transformed data using pandas: formatting date fields, calculating RFM scores, generating transaction-item matrices.

2. **Frequent Itemset & Association Rule Mining**  
   - Applied algorithms (e.g., Apriori/FP-Growth) to identify frequent item sets and generate association rules. 
   - Calculated key metrics such as support, confidence, and lift for each rule.

3. **Customer Segmentation (RFM Analysis)**  
   - Computed Recency, Frequency, and Monetary (RFM) scores in pandas.  
   - Clustered customers into segments (e.g., High Value, Occasional, Dormant) using k-means or hierarchical clustering.

4. **Visualization & Interpretation**  
   - Created visualizations using matplotlib/seaborn (and optionally Plotly) to illustrate heatmaps of associations, item-set network graphs, customer segment profiles.  
   - Derived strategic insights and actionable recommendations based on the patterns and segments uncovered.

---

## Skills:
**Programming Language:** Python  
**Libraries & Tools:** pandas, NumPy, mlxtend (for association rules), scikit-learn (for clustering), matplotlib, seaborn, Plotly  
**Techniques:** Market Basket Analysis, Association Rule Mining, Frequent Itemset Discovery, RFM Analysis, Customer Segmentation  
**Business Concepts:** Cross-sell and upsell strategy, product bundling, customer lifetime value, merchandising optimization

---

## Results & Business Recommendations:  

### 1. Product Combination Insights  
An item-set analysis revealed high-support and high-lift combinations such as *{Product A, Product B} → Product C*, indicating customers who buy A and B are highly likely to also buy C.  
Based on these findings:  
- Recommend creating **bundle promotions** for the strong item-sets.  
- Reconfigure product placement (both online and in-store) to highlight these combinations.  

### 2. Customer Segment Profiles  
Through RFM segmentation, we identified a “High Value” cluster (top 10 % of recency + frequency + monetary) that contributed disproportionately to revenue.  
Recommendations:  
- Target this cluster with **exclusive offers** and loyalty programs.  
- For “Occasional” buyers, deploy **reactivation campaigns** with targeted product-bundle suggestions based on recommendation rules.

### Summary of Insights:  
- **Frequent itemsets** provide clear cross-sell and bundling opportunities.  
- **RFM-based segmentation** enables differentiated marketing and product strategy.  
- **Association rules** support structured merchandising and campaign design.  

---

## Business Impact:
- Enhanced cross-sell potential through data-driven product bundle creation.  
- Improved marketing efficiency by focusing on high-value customer segments.  
- Strategic merchandising aligned with actual purchase behavior rather than intuition.  

---

## Next Steps:  
- Deploy a **real-time association rule engine** for live transaction monitoring.  
- Integrate product recommendations into the **e-commerce checkout experience**.  
- Extend the analysis to include **temporal patterns** (day/time of purchase) and **channel behavior** (online vs offline).  
- Use **Graph databases** or **network visualization** for richer item-relationship mapping.  

---

## Tools & Architecture:  
**Language:** Python  
**Data:** CSV transactional datasets  
**Libraries:** pandas, NumPy, mlxtend, scikit-learn, matplotlib, seaborn, Plotly  
**Visualization:** Static and interactive charts for item-set relationships and customer segmentation  
**Workflow:** Jupyter Notebook analysis, model output saved for downstream use  
**Storage:** Local CSV and output files (association rules, segment profiles)  

---

## Author:
**Aurel Sahiti**  
Data Science Graduate Student | Customer Analytics & Data Mining  
[LinkedIn](https://linkedin.com/in/aurelsahiti) | [GitHub](https://github.com/aurelsahiti)
