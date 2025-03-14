# The Cost of My Screen Time – Does More Screen Time Mean More Spending?

## Project Idea and Motivation 

This project analyzes the relationship between screen time and spending habits, specifically whether longer phone usage leads to higher spending. Many people spend hours on their phones daily, often switching between social media, shopping apps, and entertainment platforms. This study seeks to determine whether digital habits influence financial behavior by tracking daily phone usage and purchase patterns.

I decided to work on this project because I have noticed that I spend a significant amount of time on my phone, and during that time, I often end up making purchases online. This made me question whether there is a real correlation between screen time and spending habits.

Nowadays, many people are over-consuming products, especially through online shopping, food delivery, and digital subscriptions. Social media ads, instant purchases, and impulsive decisions contribute to excessive spending. I want to analyze my own habits to see if more time on my phone leads to higher spending and whether certain apps or times of day influence these behaviors.

The insights from this project could help in understanding how digital habits contribute to unnecessary spending and whether reducing screen time could improve financial awareness and self-control.

## Description of Dataset
- **Total Screen Time (hrs):** The total daily phone usage recorded from Screen Time (iOS).
  
- **Time on Shopping Apps (mins):** Time spent on apps like Amazon, eBay, and food delivery services.
  
- **Time on Social Media (mins):** Time spent on Instagram, TikTok, YouTube, and other social media platforms.
  
- **Money Spent (TL):** The total amount spent online each day.
  
- **Purchase Type:** Whether the expense was on shopping, food delivery, entertainment, or subscriptions.
  
- **Time of Purchase:** When the spending occurred will be divided in 4 sections (morning, afternoon, evening, or late night).
  
- **Ad Exposure Before Purchase:** Whether an online ad appeared before making a purchase (Yes/No).


## Plan
### Data Collection
For this project, I am collecting my own personal data over a period of several weeks. The data sources include:

- Phone Usage Data: Collected using Screen Time (iOS) to track my total screen time, app usage, and time spent on shopping and social media apps.

- Spending Data: Logged daily from bank transactions and order receipts to record the amount spent, type of purchase, and time of purchase.

- Ad Exposure Tracking: Manually recorded when I see an advertisement before making a purchase to analyze whether ads influence my spending behavior.

- Time of Purchase: Categorized as morning, afternoon, evening, or late night to check if purchases are more frequent at specific times.

- By combining these data points, I aim to analyze whether more screen time leads to higher spending, identify patterns in my digital habits, and understand if reducing screen time can help manage spending behavior.

### Data Sources

- **Phone Screen Time Data:** Collected from iOS Screen Time or Android Digital Wellbeing.
  
- **Spending Data:** Collected from bank transactions and app order histories.
  
- **Ad Tracking:** Logged manually before major purchases.

To ensure consistency and minimize bias:

- Data will be recorded daily.
  
- Unusual spending (e.g., gifts, one-time large purchases,lending money) will be flagged.
  
- External factors (sales events, holidays, etc.) will be considered.


## Data Preparation and Analysis

### Data Cleaning

- Convert date and time formats to standard datetime objects.
  
- Remove outliers (one-time large purchases that may skew results).
  
- Apply categorization encoding for purchase types and time of purchase.

### Exploratory Data Analysis 

- Histograms for total screen time and spending distribution.
  
- Boxplots to visualize spending trends across different time periods.
  
- Scatter plots to observe potential correlations between screen time and money spent.

### Hypothesis Testing

- **Null Hypothesis (H₀):** Screen time does not significantly impact spending behavior.
  
- **Alternative Hypothesis (H₁):** More screen time leads to higher spending.

I will test these hypothesis and with the data I collected over time I will conduct result based on my project in the next steps.
