# Telco Customer Churn Analysis

## Introduction

Telco companies face a significant challenge in reducing customer churn, which leads to substantial costs and revenue loss. Customer churn, or attrition, refers to customers leaving the service for various reasons. Understanding and mitigating churn is crucial for maintaining a healthy customer base and ensuring business growth. This case study aims to identify key drivers of customer churn for a fictional telco company operating in California during Q3.

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346.svg?style=for-the-badge&logo=Microsoft-Excel&logoColor=white) 
![Pivot Table](https://img.shields.io/badge/Pivot%20Table-217346.svg?style=for-the-badge&logo=Microsoft-Excel&logoColor=white)


## Objective

The primary objective of this analysis is to identify factors influencing customer churn, enabling the telco company to develop targeted retention strategies. By leveraging demographic, location, service-related, and satisfaction data, insights into customer behavior and preferences will be gained to reduce churn rates.

## Data Overview

- **The Telco customer churn data module is composed of 5 tables:**

    - Demographics
    - Location
    - Population
    - Services
    - Status

- **These tables are separated into multiple files:**

    - ```Telco_customer_churn_demographics.xlsx```
    - ```Telco_customer_churn_location.xlsx```
    - ```Telco_customer_churn_population.xlsx```
    - ```Telco_customer_churn_services.xlsx```
    - ```Telco_customer_churn_status.xlsx```
      
##  The Uml Diagram:
![image](https://github.com/Abdelrahman-Hatem/Excel-Project-Telco_customer_churn/assets/60587162/76cb6a1c-25c2-40cf-ab45-1cc1908256f9)

## Methodology

1. **Understanding Distribution**
   - Explanation of "Churned," "Joined," and "Stayed" statuses.
   
2. **Churn Categorization**
   - Analysis of churn reasons and categories provided by departing customers.
   - Percentage distribution of churn across categories.
   
3. **Geographical Impact**
   - Analysis of customer churn based on location (city).
   - Exploration of regions with higher churn rates and correlations with churn reasons.
   
4. **Demographic Analysis**
   - Exploration of the influence of demographics (gender, age, senior citizen status) on churn.
   - Identification of patterns among customers with higher churn rates based on demographic characteristics.
   
5. **Service Subscription Patterns**
   - Evaluation of the impact of various services on churn, including contract duration, payment method, and offers.
   
6. **Satisfaction Score and Churn Score**
   - Examination of the relationship between satisfaction scores and churn rates.

## 1 - Calculating Churn
  What does the "Churned," "Joined," and "Stayed" terminology represent in the context of customer status?
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/5207d3e3-821b-4aa4-994e-e039a2cc3197)

![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/2ed740ac-c8a8-412d-b7cf-54667653109e)

The overall churn rate stands at 26.54%, a figure that appears relatively elevated.


## 2 - Churn Categorization:

- Analyze the reasons behind customer churn by exploring churn reason and reasons provided by departing customers.
  

![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/07b0053b-e179-42cb-9faf-df68de1421da)

![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/986ee036-697d-418d-9a77-b0790baee54c)

The top three reasons are:
- Competitor made better offer
- Competitor had better devices
- Attitude of support person

### Take a closer look by analyzing the percentage distribution of churn across various categories.
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/a538a460-a973-4a4c-a489-a4baf1782b6e) 
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/25996993-9481-4c4b-aaa8-9ac25346464d)

- Close to half of the customers who are churning can be attributed to the competitor category.

## 3 - Geographical Impact:
- Analyze specific regions exhibit higher churn rate.
  
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/e0c54cab-28b5-41a7-8093-2ca14bfc15ae)

![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/7cf6f218-e572-43ed-8da9-f26f1ec29fe4)

- We see the largest number of customers churn in the San Diego counted 185, then Los Angeles counted 78.


### Take a closer look by exploring churn reasons provided by departing customers in the San Diego city.
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/1dc8bd0d-1e35-4372-8b72-18adc143b43e)

- Approximately 79% of customers churned due to the competitor offering a more attractive deal.
  
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/985519fd-bf08-4e14-920b-1b89d13f8317)

- will Examine in detail the reasons for churn  by Contract type and type of offers
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/a0396a9c-49b7-4f6c-9f6a-afae15e610f5)

Approximately 65% of customers churned month-to-month contracts and Offer E will most common in this city  


## 4 - Demographic Analysis: 
- I am creating a new column named "Classify age " to analyze classified demographic characteristics linked to age. The IF() method will be employed to generate a column with three distinct categories.  
   1  -  Adolescents
   2  -  Middle-Aged Adults
   3  -  senior

- Generate an additional column named "Customer Status" to analyze the classified status of customers, distinguishing between those who are still clients and those who have churned.


![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/694f0013-6f52-427c-818e-56bf40695098)

![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/f6df5531-9c1a-4f36-ad8d-6440720f22c9)

- The count of churn for  Middle-Aged Adults is around 1051 that appears relatively elevated.

- The churn rate for senior citizens exceeds the average by approximately 18%.

## 5 -  Service Subscription Patterns:
### Payment Method:
- Analyze the impact of payment method to have churn customer?
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/748ad5b9-e223-4183-9259-152c782cb03d)
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/388d0586-890f-4333-8391-f1a7852ea639)

- Bank Withdrawal stands out as the primary payment method for both churned and retained customers, emphasizing its widespread usage.
- Credit Card usage exhibits a significant churn rate, signaling a potential area for improvement and targeted retention strategies.
- Although its lower usage, Mailed Checks noteworthy churn rate raises concerns and warrants further examination.
  
- To address challenges related to Bank Withdrawal, such as delays or high fees, the company should enhance communication with banks and explore alternative solutions. The introduction of online payment options, along with incentives for their
utilization, holds promise for enhancing overall customer retention. This proactive approach is especially crucial in mitigating churn associated with Bank Withdrawals and addressing the identified concerns with Credit Card usage.

### Contract Distribution 
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/c4b9c28f-63ad-4f0b-85a7-f4ce828c6897)
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/17beb92d-6afc-4bd0-9676-65a0c290baa3)


- 100% Stacked Bar Chart by Contract And Churn Label

![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/b677f091-5630-474d-8db4-354185101e40)


![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/1236f5a9-1e71-4b24-aa2d-fd188ea52b1c)


- The highest churn rate, reaching 46%, is observed among customers with month-to-month contracts, indicating that 46% of customers under this contract type discontinued the service. In contrast, the churn rate is lower for one-year contracts, standing at 11%, and even lower for two-year contracts, with a rate of 2.5%


### Satisfaction Score and Churn Score:
- Examine the relationship between satisfaction scores and churn rates?
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/5761c895-6079-49ac-a602-2b319bd0a4db)

#### Overall Insights:
- The cumulative satisfaction scores for stayed customers far outnumber those of churned and joined customers.
- The concentration of lower scores among churned customers highlights potential areas of concern or improvement in service quality.
- The positive satisfaction distribution for joined and stayed customers indicates a generally content customer base in these categories.

#### What is the overall distribution of customer status (Churned, Joined, Stayed) across different types of offers and Which offer has the highest and lowest overall customer count?
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/1089636f-24a3-482c-a008-03f0eb99a0fb)
![image](https://github.com/Abdelrahman-Hatem/Telco_customer_churn/assets/60587162/e8fc63aa-a7f0-42e9-a216-092660a2586a)


#### Overall Insights:
- Offers B and D seem to have a higher presence among both joined and stayed customers.
- Offer E stands out as having a notable impact on churn.

## Results:

#### Understanding Distribution:
The three-month customer data indicates significant dynamics within the company's customer base:
- **Churned Customers**: Account for 26.54% of the total customer base, indicating a notable departure rate.
- **New Customer Acquisition**: Stands at 6.45%, indicating some growth in the customer base.
- **Staying Customers**: Represent the majority at 67.02%, reflecting a stable core customer base.

#### Churn Categorization:
- **Competitor Category**: Close to half of the churned customers can be attributed to competitors, indicating strong competition in the market.
- **Primary Reasons for Churn**:
 - The competitor made a better offer.
 - The competitor had better devices.
 - Attitude of support person.

#### Geographical Analysis:
- **Regions with Higher Churn**: 
  - San Diego: 185 churned customers.
  - Los Angeles: 78 churned customers.
  - Indicates areas where churn is more prevalent, potentially influenced by local market dynamics or competition.

#### Demographic Impact:
- **Payment Method**:
  - **Bank Withdrawal**: Dominates as the primary payment method for both churned and retained customers, highlighting its widespread usage.
  - **Credit Card Usage**: Exhibits a significant churn rate, suggesting potential areas for improvement and targeted retention strategies.
  - **Mailed Checks**: Despite lower usage, noteworthy churn rates raise concerns and require further examination.


#### Contract Impact:
- Customers with month-to-month contracts exhibit the highest churn rate at 46%, indicating a significant proportion of churn among this group.
- Churn rates decrease for longer contract durations, with one-year contracts at 11% and two-year contracts at 2.5%.

#### Satisfaction Score and Churn Score:
- Cumulative satisfaction scores are higher among stayed customers compared to churned and joined customers.
- Lower satisfaction scores are concentrated among churned customers, indicating potential areas for service quality improvement.

## Recommendations:

#### 1. Targeted Marketing:
- **Develop Targeted Campaigns:** Create marketing campaigns tailored to high-churn regions, leveraging insights from geographical analysis. Personalized offers and promotions can incentivize customers to stay and attract new ones.
- **Segmented Messaging:** Segmented Messaging: To guarantee relevancy and efficacy, divide up client communications based on demographics, preferences, and historical activity.

#### 2. Enhanced Customer Engagement:
- **Improve Customer Support:** Investing in the training of customer care representatives and setting up effective routes of communication will improve customer support services. Customer satisfaction can be considerably increased by promptly resolving issues.
- **Loyalty Programs:** Introduce loyalty programs to reward long-term customers and encourage retention. Exclusive perks and benefits can incentivize customers to remain loyal to the brand.
- **Personalized Service Bundles:** Offer personalized service bundles tailored to individual customer needs and preferences. Providing flexibility and customization can enhance perceived value and reduce churn.

#### 3. Regular Customer Feedback:
- **Implement Feedback Mechanisms:** Establish channels for gathering regular feedback from customers, such as surveys, feedback forms, or interactive platforms. Actively listen to customer concerns and suggestions to identify areas for improvement.
- **Adaptation to Evolving Needs:** Continuously monitor and adapt to evolving customer needs and preferences. Stay agile and responsive to market trends and changes in customer behavior to maintain competitiveness.


## Conclusion:

This case study provides a comprehensive analysis of customer churn in a fictional telco company, offering actionable insights for reducing churn rates. By understanding the interplay of demographics, location, services, and satisfaction metrics, the telco company can strategically position itself to enhance customer retention, fostering long-term success in a competitive market.


