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
  
- **Purchase Type:** Whether the expense was on shopping, market delivery, food, or beverages.
  
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
  Pearson correlation coefficient: 0.33
  P-value: 0.0007-> Statistically significant at α = 0.05.

 Time of Purchase vs. Spending:
  A boxplot showed nighttime purchases had the highest median and maximum spending.
  Morning and afternoon purchases were lower and more consistent in amount.

 Purchase Type vs. Screen Time:
  Focused analysis on "Shopping" purchases revealed a moderate correlation with screen time.

 This suggests shopping screen time  may play a bigger role in influencing purchases.

### Multivariate Insights

  -Purchase Context (Ad Exposure + Time of Purchase):
      Combining both variables showed that ad exposure at night led to the highest spending peaks. This context indicates impulsive behavior influenced by digital marketing during relaxed hours.


## Findings

  There is a statistically significant positive relationship between phone screen time and money spent, in other words it is            concluded that we can reject the null hypothesis .
  Ad exposure and late-night usage tend to amplify spending behavior. Also among the purchase type categories Shopping, Beverage,Food   and Market Deliveries; shopping has the highest correlation coefficient with the smalest p-value( which can be seen on the python     file).
  Purchases made at night were consistently higher in amount, suggesting possible impulsivity or decision fatigue.

 ## Limitations

  Self-reported data introduces potential bias or recording errors, especially for ad exposure and time of purchase.
  Sample size was limited to ~102 daily entries(it was nearly 60 before machine learning part,now it is updated to 102), making it difficult to generalize findings to wider populations.
  No demographic variation — data is based on one individual’s behavior.

## Future Work

  -Incorporate automated data extraction from device screen reports and online banking.
  
  -For the Machine Learning part I will log in more data to enrich my data set.I will also be doing different ML methods and compare each of them before finding the best model.

## Machine Learning
  Machine Learning Analysis

This section applies machine learning classification models to predict the Purchase Type based on digital usage behavior and contextual features.

Objective
Classify each spending instance into one of the following categories:

Beverage
Food
Market Delivery
Shopping




Features Used


The models are trained on the following input features:

Total Screen Time of Phone (mins)
Time on Shopping Apps (mins)
Time on Social Media (mins)
Ad Exposure Before Purchase (Yes/No)
Spending Rate
Is_Weekend




One-hot encoded: Time of Purchase (morning, evening, night)
Models Implemented
Logistic Regression
Random Forest Classifier
Data Splitting


The dataset was split into training and testing sets using an 80/20 ratio.
Stratified sampling was applied to preserve the distribution of the target variable (Purchase Type).
Evaluation Metrics


Model performance was evaluated using:

Accuracy
F1 Score (Weighted Average)
F1 Score (Macro Average)
These metrics account for class imbalance and provide insight into both overall and per-class performance.

Results Summary
Model	Accuracy	F1 Score (Weighted)	F1 Score (Macro)
Logistic Regression	0.86	0.82	0.69
Random Forest	0.67	0.67	0.56
Classification Reports
Logistic Regression

Accuracy: 0.8571
F1 Score (weighted): 0.8161


Interpretation
Logistic Regression consistently outperformed Random Forest across all metrics.
Logistic Regression achieved a higher overall accuracy (0.86 vs 0.67) and better balance across classes, particularly underrepresented ones.
Both models struggled with class 2 (Market Delivery), likely due to sample imbalance.
The final model selected for reporting and interpretation is Logistic Regression due to its superior performance and interpretability.
## Conclusion

The hypothesis was supported by the data: increased screen time is associated with higher spending, especially when combined with ad exposure and evening or nighttime phone use.

Although it was a problem of mine, this is a 21. century issue becoming more and more serious.This project demonstrates how personal digital habits can be linked to financial behavior and offers insight into the subtle ways that attention, advertising, and time of day affect our decisions but with awareness, we can intervene. I was very curious about my spending habits because of the online purchases I made and this project became and eye opener to my own habits.
