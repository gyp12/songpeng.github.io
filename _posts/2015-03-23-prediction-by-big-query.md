---
layout: post
title: "Prediction by Big Query"
description: ""
category: [Bayesian stats, Machine learning]
tags: []
---
{% include JB/setup %}

Recently several papers talked about using the queries data from the search engine (such as Google, Baidu) to predict the socks or fluenze.

1. How did it work?
2. Is it reliable?
3. What can we learn from them?
4. Are new statistic methods or computational algorithms are needed in this direction or in the future?

##Case One: relating the trading behavior with the query data##

Preis, T. _et.al.,_ (_Scientific Reports_, 2013) related the trading behavior in finalcial markets with the data from Google Trends. *Google Trends* is the place where you have the access to get the aggregted information on queries (the items people search on Google). You could easily have a look at how the volumns of different items, such as a specific movie or a famour book, is changing over the time. Then they constructed a stragety to see if these data could be used to predict the finalcial behaviour. 

> **The strategy** (_a rough description_):  
<!--- > Identify the terms with either positve or negative correlations with the changes of stock price. -->
> Given a term, if the search volume is relatively increased, they would sell the **DJIA** (*Dow Jones Industrial Average*) soon, otherwise they would buy back.

For a given term, if this strategy helps them earn more than the simple stragy only based on **DJIA** without the *Google Trends* data, we call the term has a positive influence, or otherwise. Following the strategty above, they identified  some terms, such as **debt, color, unemployment**, have positive influences on their investment strategy, while, some terms, such as **freedom, kitchen, ring**, have negative influences on their investment strategy.

##Case Two: relating the influenza epidemics with the query data##
Ginsberg, J. _et.al.,_ (_Nature_, 2009) tried to help the early detection of the seasonal influenza epidemics by the query data on *Google*. From 50 million (wow~) queries people usually used, they identified 45 queries which were most related with the influeza-like symptoms data from the public health. The queries can be classified as symptoms of an influenza, cold/flu remedy, and so on. A linear model was then fitted by integrating these queries.  The significant contribution of this work is that it can predict the influenza epidemics two weeks earlier than the traditional methods does, which enables public health officials to respond quickly. Note some also use the Baidu (one of the three largetst IT companies in China) query data to predict the same thing in China since Google is lack of these data (The reason is obvious...). 

##Discussion##
Are these works reliable, not only the methods they use, but also the way they treat the questions? From my personal opinion, the first one might not work in reality as well as they stated since you'd better keep it as a secret if you really could make it! Well, the second one seems to be reasonable. The key problem is that whether we can smell the scent by the query data before it really happens and how sensitivity it is. The latter work provides a much faster way to collect the data than the traditional methods. But the query data might be not so sensitive enough to help us predict the socks immediately.

But these works are important and interesting. They are the frontiers on the so called *Big Data*. They also let us consider some aspects on statistics. For example,

1. How to quickly detect the related variables from millions of variables?  
2. How to construct the **knowledge tree** among these variables?  




