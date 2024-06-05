# Probability Series (Part-1)

Hallo! In this series, I will write about some important concepts in probability, especially those directly related to deep learning.

## Motivation
The main reason I'm blogging about this is simple. I took the Deep Unsupervised Learning course by the Pieter Abbeel team, and in the first lecture, I was intimidated by this scary math notation (see below) :D !  But I'm definitely motivated to understand all the concepts.

**Maximum Likelihood**

"*Given a dataset* $\mathbf{x^{(1)}},...,\mathbf{x^{(n)}}$, *find* $\theta$ *by solving the optimization problem*"

```math
\arg \min_{\theta} \mathcal{L}(\theta, \mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}) = \frac{1}{n} \sum_{i=1}^n -\log p_{\theta}(\mathbf{x}^i)
```
Reading that equation, I thought, "What the heck is going on?" Why is there a log term?

**KL Divergence**
Maximizing likelihood is equivalent to minimizing KL-Divergence. Why? How's the proof? What's KL Divergence?

Based on the snippet of the lecture above, there are several concepts that need to be understood:
* *Probability Distribution*
* *Expectation*
* *Maximum Likelihood*
* *KL Divergence*

Therefore, in this post, I will explain my understanding of these probability topics in detail.

## Probability Distribution - The main Idea
In this first post we're going to talk about probability distribution




