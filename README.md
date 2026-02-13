## 📊 Market Basket Analysis with Python – eBay
📌 Brief Introduction

This project focuses on analyzing eBay customer purchasing behavior and engagement patterns using Python. By combining data cleaning, exploratory data analysis (EDA), customer segmentation, and market basket analysis, the project uncovers product affinities, behavioral segments, and factors influencing customer satisfaction and trust in recommendations.

The goal is to generate actionable business insights that can help improve personalized recommendations, cross-selling strategies, and customer retention.

## 🧠 Detailed Project Analysis
1️⃣ Project Objective

The primary objective of this project is to understand:

How customers shop and browse on eBay

Which product categories are frequently purchased together

How customers respond to personalized recommendations

What factors influence satisfaction, trust, and engagement

The analysis aims to support data-driven decision-making for marketing, recommendation systems, and inventory planning.

## 2️⃣ Dataset Overview

The dataset represents customer survey and transaction-level behavior, including:

Demographics (age, gender)

Purchase frequency and categories

Browsing patterns and device usage

Cart behavior and abandonment reasons

Review reliability, helpfulness, and rating accuracy

Shopping satisfaction and recommendation engagement

Multi-label fields such as Purchase Categories were handled carefully to preserve analytical accuracy.

## 3️⃣ Data Cleaning & Preparation

Key preprocessing steps included:

Removed duplicate and inconsistent survey responses

Handled missing values across categorical and numerical fields

Standardized categorical values (Yes / No / Sometimes, frequency levels)

Converted rating-related columns into proper numeric formats

Extracted time-based features from timestamps (Year, Month, Weekday)

Transformed multi-category purchase data using explode() for category-level analysis

Encoded ordinal variables to enable clustering and correlation analysis

This ensured the dataset was analysis-ready and reliable.

## 4️⃣ Exploratory Data Analysis (EDA)
👥 Customer Demographics

Analyzed age and gender distribution to understand the customer base

🛒 Purchase Behavior

Customers frequently purchase from multiple categories

Most popular categories identified:

Clothing & Fashion

Groceries & Gourmet Food

Home & Kitchen

Beauty & Personal Care

This indicates strong cross-category buying behavior.

🌐 Browsing Behavior

Majority of customers browse occasionally rather than frequently

Highlights potential to increase engagement through personalization and reminders

😊 Shopping Satisfaction

Average satisfaction is moderate (~3/5)

Satisfaction levels are evenly distributed, suggesting mixed experiences

Satisfaction is influenced by multiple factors, not recommendations alone

## 5️⃣ Recommendation & Review Insights

Engagement with personalized recommendations is inconsistent

“Sometimes” is the most common response, showing relevance gaps

Trust in recommendations is cautious and evenly split between “Yes” and “No”

Customers who trust recommendations show slightly higher satisfaction

Review reliability has a stronger impact on rating accuracy than review helpfulness

This highlights the importance of credible reviews in building customer trust.

## 6️⃣ Customer Segmentation (Clustering)

Using purchase frequency and shopping satisfaction, customers were segmented using K-Means clustering (K = 3):

High Engagement Customers
Frequent buyers with high satisfaction

Moderate Engagement Customers
Occasional buyers with average satisfaction

At-Risk Customers
Low satisfaction and/or low engagement

The choice of K=3 was made for business interpretability rather than over-segmentation.

## 7️⃣ Market Basket Analysis

Applied Apriori Algorithm for association rule mining

Identified frequently purchased product combinations

Revealed potential cross-selling and bundling opportunities

Helped understand product affinity patterns beyond individual categories

## 8️⃣ Visualizations Used

Bar charts for purchase categories and browsing frequency

Pie and bar charts for satisfaction distribution

Heatmaps for correlation analysis

Scatter plots for customer clusters

These visualizations made insights easy to interpret and business-ready.

## 9️⃣ Key Business Recommendations

Improve recommendation relevance using browsing and purchase history

Apply segment-based personalization for different customer groups

Increase transparency by explaining why products are recommended

Prioritize products with reliable and verified reviews

Use feedback loops to refine recommendation quality

## 🛠️ Tools & Technologies

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Apriori Algorithm (Market Basket Analysis)
