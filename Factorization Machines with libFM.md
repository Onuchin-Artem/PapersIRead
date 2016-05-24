In this article I'm going to summarise paper ["Factorization Machines with libFM"](http://www.csie.ntu.edu.tw/~b97053/paper/Factorization%20Machines%20with%20libFM.pdf) of Steffen Rendle, 2012.
In this paper Steffen overviews state of art in Factorization Machines research at that moment.
Factorization macines is an approach in supervised machine learning that combines 
flexibility of feature engineering with power of matrix factorization.
I found that this approach is very popular in kaggle community specially in challenges like ctr-prediction 
that's why I decided to study it better.

Also this paper repeats in a lot Steffen's original paper where he defines Factorization Machines for the first time so I will refer original paper as well. 

Motivation
==========

Let's take a look at a typical process of improving machine learning systems.
Usually, there is a general supervised learning algorithm, for example SVM, depolyed to production. And a lot of efforts are usually put into feature engineering - process of converting raw data into real values matrix. According another great paper  feature engineering is the key in machine learning.
And if you think you can find that feature engineering is really powerfull technique: you don't have to change model to imrove it - it means you don't have to rewrite the whole system; you always can incomporate new data source into existing model through feature engineering.

On the other hand in recomendation systems domain, very specialized unsupervised models like matrix factorization are widely used. These models are really great in analyzing hidden interactions between categorical features - e.g. users and movies in movies recomendation system. 
-Something about predicting unseen interactions.

The problem with these factorization approaches is that they usually work with very specific input data. That's it: if you want to build a 
system that recomends movies to users based on information whether they like these movies or not you take one model. If you want to use rating data as well you take a different one, if you want to use time data you take a third one.

So, Steffen Rendle invented a way to combine flexibility of feature engineering with matrix factorization's ability to learn hidden interaction between categorical variables. This way is object of paper we going to discuss.

Paper structure
===============

This paper consists of intruduction, conclusion and four parts:

- Factoriation machine model. In this part author mathematically defines what factozation machine is.
- Learning factorization machines.
- Related work and application of factorization machines.
- Evaluation.

What is factorization machines?
===============================

Train Approaches
================

Relationship to other models
============================

Implemenations overview
========================

Summary
=======

