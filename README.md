# Sport Center Market Research : Project Overview

DQLab sports center is a store that sells various sports needs such as Jackets, Clothes, Bags, and Shoes. This store started selling since 2013, so it already has regular customers for a long time, and is still trying to get new customers until now. In early 2019, the store manager recruited a junior DA to solve their problem,that is decreasing customers who buy back into the store. The Junior DA was also entrusted to processing the store's transaction data. The store manager defines that the customer is no longer called a customer (churn) when they have not transacted to the store again until the last 6 months from the last data update. The store manager also provided transaction data from 2013 to 2019 in csv form (comma separated value) named data_retail.csv with 100,000 rows of data.

(Both case study and dataset are provided by dqlab.id)

## Early Insight from Data
- Customer acquisition by year :  we want to see trend of acquisition by year.
![alt_text](https://github.com/annisahumaira21/sport-center-market-research/blob/main/customer%20acqusition%20by%20year.JPG)

 Customers who transact increases every year, then total customers decreases slightly in 2018 and 2019.
 
- Transaction by year

![alt_text](https://github.com/annisahumaira21/sport-center-market-research/blob/main/Transaction%20Customer.JPG)

  transactions tends to increase until 2017 and decreases in 2018 and 2019
  
- Average transaction amount by year

![alt_text](https://github.com/annisahumaira21/sport-center-market-research/blob/main/Average%20Transaction%20Amount%20by%20Year.JPG)

  the average transaction for jackets and shoes was quite stagnant, but for clothes and bags significantly increased until 2018 and began to decline in 2019.
    
- Proportion of churned customer for each product

![alt_text](https://github.com/annisahumaira21/sport-center-market-research/blob/main/Proportion%20of%20Churned%20Customer%20for%20each%20product.JPG)

  as we can see, the number of churn customers is quite a lot, above 60% for each product.
    
- Customer Distribution by Count Transaction Group

![alt_text](https://github.com/annisahumaira21/sport-center-market-research/blob/main/Customer%20Distribution%20by%20Count%20Transaction%20Group.JPG)

  Most of customers only buy 1 product.
    
- Customer Distribution by Average Transaction Amount Group 

![alt_text](https://github.com/annisahumaira21/sport-center-market-research/blob/main/Customer%20distribution%20by%20average%20transaction%20amount%20group.JPG)

  From the graph above, it turns out that most customers have a fairly large number of transactions, 1 million- 2.5 million
    
## Modelling

by using Logistic Regression, results of model evaluation are shown below 
Eval Model | Accuracy | Precision | Recall  | F1 Score | AUC |
| -- | -- | -- | -- | -- | -- |
Score | 0.77 | 0.78 | 0.92 | 0.84 | 0.69 |

evaluation model used is F1 Score because it's suitable for unbalanced target data. from model evaluation, the results of F1 score are quite good at 0.84.

## Conclusion and Recommendation
- trend the number of customers increasing every year until 2017 and then starting to decline until 2019
- the number of transactions also tends to increase every year, but has decreased significantly in 2018 and 2019
- most customers only buy 1 product but with a price range of 1 million-2.5 million
- the percentage of customers who churn above 60% in each product.
- From the results above, recommendations can be made:
  - stores can collect customer data that is predicted to churn early so discounts or attractive promos can be given to keep customers from churn and continue to transact.
