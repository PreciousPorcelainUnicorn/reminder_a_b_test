# reminder_a_b_test
# Pinned Reminders A/B Test Analysis

## Project Overview
This project evaluates the performance of a newly implemented feature: pinned reminders for users with 5 or fewer credits remaining on their account. The feature is designed to target highly engaged users, reminding them to replenish their balance to continue using the platform.
The objective of this analysis is to determine whether introducing pinned reminders results in a statistically significant lift in the First-Payment Conversion Rate (CR) among the target audience.

## Project Structure & Workflow
1. **Pre-Analysis & Baseline Determination (Historical Data)** \
Target Audience Definition: Filtered historical data to isolate users who spent at least 15 credits (the necessary milestone where the feature could actively trigger). \
Baseline Calculation: A historical conversion rate of 14.38% for the target user segment. \
Sample Size & Duration Planning: Using a 10% Minimum Detectable Effect (MDE), 80% power, and a significance level of alpha = 0.05, the minimum required sample size was determined to be 9,460 users per group. \
Given an average number of 2,474 target users/day, a minimum runtime of 8 days was set to ensure sufficient data was collected.
2. **A/B Test Execution** \
The experiment was conducted with a control group (A) receiving no reminders and a test group (B) interacting with the pinned reminders. \
**Null Hypothesis:** Pinned reminders have no effect or a negative impact on the first-payment conversion rate. \
**Alternative Hypothesis:** Pinned reminders significantly increase the first-payment conversion rate. \
Methodology: Applied a one-sided Z-test of proportions along with confidence interval mapping to check statistical validity.

## Key Results 
Control Group (A): \
Sample Size - 25,695 users \
First-Payment Conversions - 3,463 users \
Conversion Rate (CR) - 13.48%

Test Group (B): \
Sample Size - 25,858 users \
First-Payment Conversions - 3,682 users \
Conversion Rate (CR) - 14.24% 
(Absolute Lift +0.76%)

The p-value from the Z-test is less than alpha = 0.05, providing robust statistical grounds to reject the null hypothesis.

## Conclusion
The feature successfully drives commercial conversion among high-intent users on the platform.

## Tech Stack & Libraries Used
Language: Python
Libraries: pandas, numpy, matplotlib, seaborn, statsmodels (Proportions Z-test & Confidence Intervals).
