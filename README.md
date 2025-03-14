# The Cost of My Screen Time – Does More Screen Time Mean More Spending?

## Project Idea
This project analyzes the relationship between screen time and spending habits, specifically whether longer phone usage leads to higher spending. Many people spend hours on their phones daily, often switching between social media, shopping apps, and entertainment platforms. This study seeks to determine whether digital habits influence financial behavior by tracking daily phone usage and purchase patterns.

## Description of Dataset
- **Total Screen Time (hrs):** The total daily phone usage recorded from Digital Wellbeing (Android) or Screen Time (iOS).
- **Time on Shopping Apps (mins):** Time spent on apps like Amazon, eBay, and food delivery services.
- **Time on Social Media (mins):** Time spent on Instagram, TikTok, YouTube, and other platforms.
- **Money Spent ($):** The total amount spent online each day (bank transaction logs).
- **Purchase Type:** Whether the expense was on shopping, food delivery, entertainment, or subscriptions.
- **Time of Purchase:** When the spending occurred (morning, afternoon, evening, or late night).
- **Ad Exposure Before Purchase:** Whether an online ad appeared before making a purchase (Yes/No).


## Plan
### Data Collection
- Data will be collected over several weeks, maintaining:
  - Consistent tracking of daily screen time and spending.
  - Detailed categorization of purchases and app usage.
  - Regular recording to ensure accurate data collection.

### Data Sources
- **Phone Screen Time Data:** Collected from iOS Screen Time or Android Digital Wellbeing.
- **Spending Data:** Collected from bank transactions and app order histories.
- **Ad Tracking:** Logged manually before major purchases.

To ensure consistency and minimize bias:
- Data will be recorded daily at the end of each day.
- Unusual spending (e.g., gifts, one-time large purchases) will be flagged.
- External factors (sales events, holidays, etc.) will be considered.


## Data Preparation and Analysis
### Data Cleaning
- Convert date and time formats to standard datetime objects.
- Remove outliers (one-time large purchases that may skew results).
- Apply categorization encoding for purchase types and time of purchase.

### Exploratory Data Analysis (EDA)
- Histograms for total screen time and spending distribution.
- Boxplots to visualize spending trends across different time periods.
- Scatter plots to observe potential correlations between screen time and money spent.

### Hypothesis Testing
- **Null Hypothesis (H₀):** Screen time does not significantly impact spending behavior.
- **Alternative Hypothesis (H₁):** More screen time leads to higher spending.
