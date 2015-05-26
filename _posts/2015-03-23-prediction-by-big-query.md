---
layout: post
title: "Prediction by Big Query"
description: ""
category: [Bayesian stats, Machine learning]
tags: []
---
{% include JB/setup %}

Recently several papers talked about prediction of the socks or the fluenza using the queries data from the search engine (such as Google, Baidu).
Then one may ask the following questions:
1. How did it work?
2. Is it reliable?
3. What can we learn from them?
4. Are new statistic methods or computational algorithms needed in this direction or in the future?

##Case One: relating the trading behavior with the query data##

Preis, T. _et.al.,_ (_Scientific Reports_, 2013) related the trading behavior in financial markets with the data from Google Trends. *Google Trends* is the place where you have the access to get the aggregated information on queries (the items people search on Google). You could easily have a look at how the volumes of different items, such as a specific movie or a famous book, are changing over the time. Then they constructed a strategy to see if these data could be used to predict the financial behaviors. 

> **The strategy** (_a rough description_):  
<!--- > Identify the terms with either positve or negative correlations with the changes of stock price. -->
> Given a term, if the search volume is relatively increased, they would sell the **DJIA** (*Dow Jones Industrial Average*) soon, otherwise they would buy back.

For a given term, if this strategy helps them earn more than the simple strategy only based on **DJIA** without the *Google Trends* data, we say the term has a positive influence, or otherwise. Following the strategy above, they identified  some terms with positive influences on their investment strategy, such as **debt, color, unemployment**. While, other terms, such as **freedom, kitchen, ring**, have negative influences on their investment strategy.

##Case Two: relating the influenza epidemics with the query data##
Ginsberg, J. _et.al.,_ (_Nature_, 2009) tried to help the early detection of the seasonal influenza epidemics by the query data on *Google*. From 50 million (wow~) queries people usually used, they identified 45 queries which were most related with the influeza-like symptoms data from the public health. The queries can be classified as symptoms of an influenza, cold/flu remedy, and so on. A linear model was then fitted by integrating these queries.  The significant contribution of this work is that it can predict the influenza epidemics two weeks earlier than the traditional methods, which enables public health officials to respond quickly. Note that some people also use the Baidu (one of the three largest IT companies in China) query data to predict the same thing in China since Google is lack of these data (The reason is obvious...). 

##Discussion##
Are these works reliable, not only the methods they use, but also the way they treat the questions? From my personal view, the first one might not work in reality as well as they stated since you'd better keep it as a secret if you really could make it! Well, the second one seems to be reasonable. The key problem is that whether we can smell the scent by the query data before it really happens and how sensitive it is. The latter work provides a much faster way to collect the data than the traditional methods. But the query data might be not sensitive enough to help us predict the socks immediately.

Anyway these works are important and interesting. They are the frontiers on the so called *Big Data*. They also drive us to consider statistics. For example,

1. How to quickly detect the related variables from millions of variables?  
2. How to construct the **knowledge tree** among these variables?  

Note:
This artical is modified at May 18,2015 under the help of Shang Su.



