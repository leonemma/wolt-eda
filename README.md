# Analyzing Wolt User Behavior

## Table of Contents
- [Overview](#Overview)
- [Goals](#Goals)
- [Data Source](#Data-Source)
- [Findings](#Findings) 
- [Key Questions](#Key-Questions)
- [Key Metrics](#Key-Metrics)
- [Summary](#Summary)
  
## Overview
This analysis focuses on user behavior and purchasing patterns within the Wolt platform during September 2019. The dataset includes 21,983 registered users, capturing their registration details, device preferences, ordering habits, and total spend. Despite high registration numbers, a significant portion of users did not place any orders, making it essential to clean a big amount of data and then investigate engagement levels. By analyzing when users order, how often and how much they spend, the goal is to uncover trends that can inform business strategies. Through visualizations and metrics, the analysis provides a comprehensive look at how customers interact with the platform.
## Goals
1. **Understand User Behavior**:
    Analyze how users interact with the Wolt platform in terms of registration, ordering frequency, and time-based activity.
3. **Identify Spending Patterns**:
    Explore how much users spend on average, segment customers based on their total purchases, and detect key trends in meal preferences.
5. **Evaluate Platform Engagement**:
    Measure how many users are active, inactive, or one-time buyers, and assess usage patterns across countries and devices.

## Data Source
The dataset used in this analysis was shared publicly by Wolt on their official LinkedIn page as part of a data challenge initiative. It contains anonymized customer-level data from the month of September 2019, intended to encourage exploration of user behavior, purchase activity, and data-driven decision making. No personally identifiable information is included, and the dataset is suitable for research purposes.

## Findings
This analysis focuses on Wolt’s customer data from September 2019, where each row represents a registered user. From our analysis we conclude: 
- There are 21983 unique registered users during this month
- Users placed 73,351 orders throughout the month
- Wolt generated approximately €2.1 million in revenue
- The average spend per user was €176.49
- The average spend per purchase was €31.10


## Key Questions
### 1. How many Wolt's users made at least one order?
   
As we see from the pie plot below, nearly half of Wolt's users made no purchase, highlighting a large inactive group.

![ActiveUsers](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/active.png)

  
Focusing on the distribution of the purchase count, we observe that only 22% of users made more than three purchases, suggesting a relatively small but highly engaged segment. Additionally, purchase activity declines significantly after the first transaction, highlighting potential challenges in encouraging repeat purchases."

  
![Purchase_Count](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/1purchase_count_final.png)


### 2. Where in the world are Wolt users?
Next, we focus on the countries where users made their purchases. As seen in the barplot, a few countries dominate user activity, reflecting Wolt’s strongest market presence.

![Country_Distribution](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/2countries_reg_final.png)  

However, we’re more interested in the proportion of active users each country has.
The following plot highlights user activity levels by country, giving insight into how engaged Wolt users are across different regions.  

![Country_Active_Ratio_distribution](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/2.2last_plot.png)

We notice that, although Finland has the highest number of users, Denmark leads in user engagement, with 61.5% of users placing at least one order. Finland follows with 53% active users, while Greece shows a balanced 50-50 split between active and inactive users. 

### 3. How does user activity evolve over time?
In the next visualization, we explore two key trends: daily user registrations and the number of purchases made per registration day. By comparing these line plots, We can see how user activity matches with purchase behavior over time, and whether days with more sign-ups lead to more purchases.  

![Daily_Registration_Purchases_LinePLots](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/new_combined.png)

### 4. When do users love to order?
To better understand user behavior, we examined the timing of purchases throughout September. The following heatmap reveals patterns across days of the week and hours of the day, helping us identify peak ordering times and potential engagement windows.  

![Heatmap](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/newplot%20(1).png)

After analyzing the heatmap alongside the countplots, we conclude that Thursday is the busiest day for Wolt. Regarding the times of high activity alongside the day of the week, we can identify blocks with the most intense blue coloring, which indicates a high number of purchases. For example, these high-activity periods occur:
- Between 16:00 and 19:00 every day except of Monday & Tuesday
- Between 02:00 and 05:00 on Monday and Tuesday
- Between 00:00 and 02:00 on Friday, Saturday & Sunday

### 5. What do users prefer?
To get a better sense of user preferences, we look at two key choices: the platform they use (Android, iOS, or Web) and their preferred order type (delivery or takeaway). The donut charts below give us a quick overview of how users interact with Wolt across these options.  

![Users_pref](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/users_pref.png)

### Key Metrics
To sum up the analysis, we define a few key metrics: 
1. The average number of daily subscribers,
2. Average daily orders
3. Average daily income in EUR.
     
These values provide a high-level overview of Wolt’s daily performance and can serve as useful benchmarks for tracking growth, identifying trends, and evaluating business health over time.

|            Metric         |   Value  |
|---------------------------|----------| 
| Average Daily Subscribers |   730.6  |
|   Average Daily Orders    | 2,445.03 |
|  Average Daily Income (€) | 70,376.5 |   


### Classifying Customers by Spending Behavior
To better understand user value, we segment customers based on their total spending (TOTAL_PURCHASES_EUR). We divide the distribution of this feature into three equal parts (tertiles):

- **Low Spenders**: Users in the lowest third of the distribution.
- **Regulars**: Users in the middle third.
- **Premium**: Users in the top third, representing the highest spenders.

Additionally, users who have never placed an order are automatically classified as Low Spenders, since they haven’t contributed any spending activity.
This segmentation helps us analyze behavior across different customer value groups and tailor insights or strategies accordingly.

![Users_Segmentation](https://github.com/leonemma/Wolt-Purchase-Behavior-Analysis/blob/main/Plots/customer_new.png)

### Summary
This analysis provided a detailed look into Wolt users' behavior, preferences, and value to the platform. By examining user activity over time, preferred platforms, order types, and spending patterns, we gained valuable insights into how users interact with the service. Segmenting customers by spending level further helped us identify key user groups—Low Spenders, Regulars, and Premium users—which can guide future marketing strategies and personalized experiences.  
- The code for this project is available [here](https://github.com/leonemma/wolt-eda/blob/main/Wolt_EDA.ipynb)

