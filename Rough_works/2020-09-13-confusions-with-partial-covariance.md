---
layout: post
usemathjax: true
title: "Precision Matrix and Partial Correlation"
date: 2020-09-13
---
One fine Sunday morning I made a rookie mistake. I was trying to study the properties of conditional distribution of a **Multivariate Normal** distribution, because, although I knew the properties their derivations were a bit rusty. Now, as I said it was Sunday morning and in my defense I was trying to work even though I was exhausted and still half asleep. Turned out that my inadequately rested brain messed up the concepts of **Partial Correlation**, **Partial Covariance** and **Precision Matrices**. So I decided to create this short write-up, so that any reader or my future self with similar dilemma can rectify their misunderstandings. Here goes:<br>
Let $$\mathbf{X} = [X_{1},X_{2},\dots,X_{p}]^{\top}$$ follow a $$p$$-variate Normal distribution with mean $$0$$ and a covariance matrix $$\Sigma$$. We will assume $$\Sigma$$ to be positive definite. Then the **Precision matrix** of $$\mathbf{X}$$ is defined as $$\Omega := \Sigma ^{-1}$$. Now we know that if we partition $$\mathbf{X} = [\mathbf{X^{(1)}}^{\top},\mathbf{X^{(2)}}^{\top}]^{\top}$$, where $$\mathbf{X^{(1)}} = [X_{1},X_{2}]^{\top}$$ and $$\mathbf{X^{(2)}} = [X_{3},X_{4},\dots,X_{p}]^{\top}$$.
