# Wolt-Purchase-Behavior-Analysis

## Table-of-Contents
- [Overview](#Overview)
- [Goals](#Goals)
- [Data Source](#Data-Source)
- [Key Questions](#Key-Questions)
- [Findings](#Findings) 

## Overview
This analysis focuses on user behavior and purchasing patterns within the Wolt platform during September 2019. The dataset includes 21,983 registered users, capturing their registration details, device preferences, ordering habits, and total spend. Despite high registration numbers, a significant portion of users did not place any orders, making it essential to investigate engagement levels. By analyzing when users order, how often they do so, and how much they spend, the goal is to uncover trends that can inform business strategies. Through visualizations and metrics, the analysis provides a comprehensive look at how customers interact with the platform — from breakfast orders to total monthly spending — helping to turn raw data into actionable insights.

## Goals
1. **Understand User Behavior**:
    Analyze how users interact with the Wolt platform in terms of registration, ordering frequency, and time-based activity.
3. **Identify Spending Patterns**:
    Explore how much users spend on average, segment customers based on their total purchases, and detect key trends in meal preferences.
5. **Evaluate Platform Engagement**:
    Measure how many users are active, inactive, or one-time buyers, and assess usage patterns across countries and devices.

## Data Source
The dataset used in this analysis was shared publicly by Wolt on their official LinkedIn page as part of a data challenge initiative. It contains anonymized customer-level data from the month of September 2019, intended to encourage exploration of user behavior, purchase activity, and data-driven decision making. No personally identifiable information is included, and the dataset is suitable for research purposes.

## Key Questions
1. How many Wolt's users made at least one order?
2. What's the average total spend per user?
3. What's the best day or hour for a purchase?
4. Where in the world are Wolt users?

## Findings
This analysis focuses on Wolt’s customer data from September 2019, where each row represents a registered user. From our analysis we conclude: 
- There are 21983 unique registered users during this month
- Users placed 73,351 orders throughout the month
- Wolt generated approximately €2.1 million in revenue
- The average spend per user was €176.49
- The average spend per purchase was €31.10



1. **How many Wolt's users made at least one order?**
   
As we see from the pie plot below, nearly half of Wolt's users made no purchase, highlighting a large inactive group.

![ActiveUsers](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/active.png)

  
Focusing on the distribution of the purchase count, we observe that only 22% of users made more than three purchases, suggesting a relatively small but highly engaged segment. Additionally, purchase activity declines significantly after the first transaction, highlighting potential challenges in encouraging repeat purchases."

  
![Purchase_Count](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/purchase_count.png)


2. **Where in the world are Wolt users?**
