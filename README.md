# Mini-Project-3: Predict Customer Personality to Boost Marketing Campaign by using Machine Learning
## Background
A company can experience rapid growth by understanding the personality traits of its customers, enabling them to provide better services and benefits to potential loyal customers. It's essential for the company to understand customer behavior to enhance marketing campaigns.
## Goal
Enhance marketing campaign performance and target the right customers for transactions on the company's platform.
## Objective
Create a predictive clustering model using unsupervised learning to facilitate decision-making for the company.
## Data Overview
The dataset consists of 2,240 rows of data and 30 customer behavior features related to transactions and interactions on our platform.
## Tools
In this project, I used Python as the programming language, Jupyter as the notebook, pandas, numpy, sklearn for preprocessing and machine learning, and a combination of matplotlib and seaborn libraries for data visualization.
## Content
### Data Preprocessing
In this section, various processes are performed, including handling missing values using MICE with Light GBM, addressing data duplicates, feature selection using LRFM method (Recency, Frequency, Monetary, Loyalty), outlier handling through manual trimming (removing values far in the year 1893-1900 in the Year Birth column and values as high as 666M in the Income column), feature transformation using Yeo-Johnson Transformation, normalization with Min-Max scaling, and feature scaling with StandardScaler.
### Data Modeling
Utilizing K-Means Clustering with cross-validation, elbow method for inertia scores, and silhouette.
### Customer Personality Analaysis for Marketing Retargeting
Based on my model, there are 4 customer groups:

**1. Cluster 0 (Loyal Customer):**
- This group is the group with the third largest number of customers, namely 550 people.
  
- Customers in this group have an average time since last purchase (22 days), and an average total purchase (21 items) which means they shopped in the near future, shopped frequently and they spent a lot of money on our platform (around IDR 919k /year).

- Customers in this group are less likely to respond to campaigns, but this group visits the website quite often with a median of 5 times a month.
  
**2. Cluster 1 (Need Attention):**
- This group is the group with the largest number of customers, 941 people.

- Customers in this group have an average time since last purchase (48 days), and an average total purchase (7 items) which means they haven't shopped for quite a while, are not regular buyers and they spend a small amount of money on our platform (around Rp. 79k/year).

- Customers in this group responded the least to the campaign but this group visited the website most often with a median of 7 times a month.
  
**3. Cluster 2 (At Risk):**
- This group is the group with the second largest number of customers, 609 people.

- Customers in this group have an average time since last purchase (73 days) which means they haven't shopped on our platform the longest compared to other groups, and an average total purchase (20 items) which means they shop frequently and spend a lot of money on the platform us (around IDR 930k/year).

- Customers in this group are less likely to respond to campaigns, but this group visits the website quite often with a median of 5 times a month.
  
**4. Cluster 3 (Potential Loyalist):**
- This group is the group with the smallest number of customers, 136 people.

- Customers in this group have an average time since last purchase (48 days), and an average total purchase (21 items) which means they shop frequently and spend the most money on our platform (around IDR 1.5 million/year) compared to the group other.

- Customers in this group responded the most to the campaign twice, but this group visited the website only 3 times a month.
### Business Recommendations

**1. Loyal Customers:**
- **Maintain Engagement:** Continue regular communication through relevant and engaging marketing campaigns.

- **Special Offers:** Give customers exclusive offers or discounts as a reward for their engagement.

- **Rewards Programs:** Consider introducing a rewards program that offers incentives for active participation and purchases.
  
**2. Need Customer Attention:**
- **Reactivation:** Send attractive offers or discounts to encourage customers to shop again.

- **Special Offers**: Provide special offers or limited discounts to stimulate further purchases.

- **Educational Content:** Send content that provides valuable information about products or usage methods to increase interest and engagement.
  
**3. At Risk Customer:**
- **Personalization Campaigns:** Strive to send more relevant and engaging campaigns to customers in this group.

- **Exclusive Offers:** Provide exclusive offers or special discounts to customers in this group. This can be an added incentive for them to shop again despite receiving infrequent marketing campaigns.

- **Loyalty Program:** Invite them to join a loyalty program that offers exclusive benefits to loyal customers.

- **Experiment with Different Media and Channels:** Try testing campaigns through different media or channels. Some customers may respond better if the campaign is delivered via email, SMS, social media, or online advertising. This experiment can help us find the most effective communication channels for this group.

**4. Potential Loyalist Customers:**
- **Personalization Campaigns:** Increase efforts to send more personalized and relevant marketing campaigns to customers in this cluster.

- **Discount Offers:** Provide special offers or discounts to customers to encourage further purchases.
Loyalty Programs: Get customers to join loyalty programs that offer additional incentives for high purchases.

- **New Product Notifications:** Inform them about new products that align with their interests and preferences.
### Potential Impact
If we can prioritize all groups and they don't churn, we still have a GMV potential of around IDR 1.3 billion/year.

Loyal Customer = IDR 505 million/year • Need Attention Customer = IDR 74 million/year • At Risk Customer = IDR 566 million/year • Potential Loyalist Customer= IDR 208 million/year.
