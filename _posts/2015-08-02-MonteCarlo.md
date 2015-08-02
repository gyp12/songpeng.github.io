---
layout: post
title: "Monte Carlo Strategies"
description: "Techniques"
category: [Bayesian Stats]
tags: []
---
{% include JB/setup %}

One of the basic and important things in Bayesian statistics is sampling, either from the posterior distribution or calculating the expectations and so on. Monte Carlo strategy are just designed for it, and it's largely depend on lots of computational simulations.

I began to learn the Monte Carlo from reading a well-written book called *Monte Carlo Strategies in Scientific Computing* by Jun S. Liu, who is the professor in the department of statistics, Harvard University.

Jun gives us the very direct and intensive explanations on Monte Carlo strategies without too many mathematical formulas. In fact, he makes a major contribution on this field. Reading this book, for me, is an quite interesting and happy things in life. But I have to say it might be a little old since it was published in 2001.

From my personal opinion,  Monte Carlo strategies can be summarized below:

> 1. Basic strategy:
    * Important Sampling
    * Rejection Sampling
    * MCMC including Gibbs sampling

> 2. Important ways:
    * Sequential Monte Carlo
    * Multiple tries when sampling.
    * Multiple chains when sampling.
    * Adding auxiliary variables, such as Hybrid Monte Carlo, Slice Sampling.
