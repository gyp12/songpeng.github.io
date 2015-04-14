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

Preis T. _et.al.,_ (_Scientific Reports_, 2013) related the trading behavior in finalcial markets with the data from Google Trends. *Google Trends* is the place where you have the access to get the aggregted information on queries (the items people search on Google). You could easily have a look at how the volumns of different items, such as a specific movie or a famour book, is changing over the time. By the help of *Google Sets* service, they identified  some terms, such as **unemployment**, have positive influences on their investment strategy, while, some terms, such as **freedom**, have negative influences on their investment strategy.

*The strategy*:
> Identify the terms with either positve or negative correlations with the changes of stock price.
> 
