# Enhancement_of_Market-Basket_Analysis_using_Topic_modeling
Initially we had a insta-cart user shopping data, so to increase their revenue we did a market basket analysis on the entire dataset which had around 50k products and 3 million orders and with 200k users there are around 32 million transactions.

So after applying Market Basket Analysis (using Apriori Algorithm) to the entire dataset, i.e all users with all their products.

As we do this, we obtain just 4 association rules and that also with a low confidence and lower lift value, But here due to computational limitations we had to lower down the support count to a very high value. But to get better rules, we thought of apply apriori algorithm to the user cluster obtained after performing LDA on the user dataset, keeping users as documents and products as words.

To do LDA on a bag of words, but here we have a bag of products instead, and after LDA we will use topic distribution to find user clusters and we will then apply Market Basket Analysis on the specific user cluster rather than on the whole data set.