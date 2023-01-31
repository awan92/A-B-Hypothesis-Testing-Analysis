# A/B Hypothesis Testing : Which one is better, The New Landing Page or The Old one?
Successfully help the company to validated whether the new landing page will give a better conversion rate before rolling out to a bigger audience. With A/B testing, the company can decide to keep using the old one because the result shows that there is no significant differences in conversion rate between the old and the new landing page.

-	Tools: Python 
- See my code [here](https://colab.research.google.com/drive/1sX9T4WyCnorV_lFtylHxLOhGzezbPIKL?usp=sharing)

## Background
An e-commerce company is revamping a new landing page. The company want to experiment whether the new landing page will give better conversion rate before rolling out to a wider audience.

## Data Overview
We were given the experiment result from control and experimental/treatment group. We have hypothesis that the new page (treatment group) will give a better conversion rate.

## Objective
To help company in deciding which landing page is better

## Exploratory Data Analysis (EDA)
Split the data into 2 groups based on this 2 condition
- **Condition 1:** control group must receive old landing page only
- **Condition 2:** treatment group must receive new landing page only

**Result:**
- The number of user in both group is quite balanced (Control group : 2505 and Treatment Group : 2438)
- The conversion rate in treatment group (new landing page) is slightly higher than the conversion rate in control group (old landing page). **But is this difference significant enough?** In order to identify the difference, **A/B hypothesis testing should be done first**

## A/B Testing
One tailed Z-test was chosen to prove the hypothesis. Either one of these statement is true for our testing result:

**Null Hypothesis (H0**): Conversion rate in new page **less than or equal to** the conversion rate in old page

**Alternative Hypothesis (H1)**: Conversion rate in new page **better than** the conversion rate in old page

## Insight and Recommendation
(Z-score = 0.578, p-value = 0.281) 

**Result:**

The p_value > 0.05, We don't have enough evidence to reject null hypothesis, thus we **accept null hypothesis**. New landing page doesn't give better conversion rate than the old one.

**Recommendation**

The company can keep using the old landing page, because the hypothesis testing result show that conversion rate in new landing page doesn't sginificantly differ with the one in old landing page.
