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

I’ll log all of this daily in an Excel file, ensuring consistent and accurate data collection.By combining these data points, I aim to analyze whether more screen time leads to higher spending, identify patterns in my digital habits, and understand if reducing screen time can help manage spending behavior.

### Data Sources

- **Phone Screen Time Data:** Collected from iOS Screen Time .
  
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



## Results of the Analysis

### Univariate Analysis

- Total Screen Time:
A histogram revealed a fairly normal distribution, with most daily screen time falling between 180–300 minutes.
Outliers at the higher end (300+ mins) suggest occasional intensive phone use.

- Money Spent (TL):
   - A histogram showed a right-skewed distribution with a small number of high-spending days.
   - The average daily spending was ₺581, with a maximum of ₺2866.

- Ad Exposure:
  Users were exposed to ads in about 45% of recorded days.

A slight increase in average spending was observed when ad exposure was present.

### Bivariate Analysis

 Screen Time vs. Money Spent:
  A scatter plot revealed a moderate positive correlation between screen time and spending.
  Pearson correlation coefficient: 0.36P-value: 0.0113 -> Statistically significant at α = 0.05.

 Time of Purchase vs. Spending:
  A boxplot showed nighttime purchases had the highest median and maximum spending.
  Morning and afternoon purchases were lower and more consistent in amount.

 Purchase Type vs. Screen Time:
  Focused analysis on "Shopping" purchases revealed a moderate correlation with screen time.

 This suggests shopping screen time  may play a bigger role in influencing purchases.

### Multivariate Insights

  -Purchase Context (Ad Exposure + Time of Purchase):
      Combining both variables showed that ad exposure at night led to the highest spending peaks. This context indicates impulsive         behavior influenced by digital marketing during relaxed hours.


## Findings

  There is a statistically significant positive relationship between phone screen time and money spent.
  Ad exposure and late-night usage tend to amplify spending behavior. Also among the purchase type categories Shopping, Beverage,Food   and Market Deliveries; shopping has the highest correlation coefficient with the smalest p-value eventhough it is 0.0566.
  Purchases made at night were consistently higher in amount, suggesting possible impulsivity or decision fatigue.

 ## Limitations

  Self-reported data introduces potential bias or recording errors, especially for ad exposure and time of purchase.
  Sample size was limited to ~49 daily entries, making it difficult to generalize findings to wider populations.
  No demographic variation — data is based on one individual’s behavior.

## Future Work

  -Incorporate automated data extraction from device screen reports and online banking.
  
  -Track purchase purpose and emotional state to understand motivational factors.
  
  -Include notifications, scrolling patterns, or ad content types for richer behavior modeling.

## Conclusion

The hypothesis was supported by the data: increased screen time is associated with higher spending, especially when combined with ad exposure and evening or nighttime phone use.

Although it was a problem of mine, this is a 21. century issue becoming more and more serious.This project demonstrates how personal digital habits can be linked to financial behavior and offers insight into the subtle ways that attention, advertising, and time of day affect our decisions but with awareness, we can intervene. I was very curious about my spending habits because of the online purchases I made and this project became and eye opener to my own habits.
