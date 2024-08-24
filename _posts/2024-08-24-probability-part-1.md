# Probability Part 1 (Motivation, Counting Methods, Basic Principles)
All credits belong to Dr. Karthik Nandakumar & Dr. Huan Xiong
## Why do we study probability theory?
We live in a world full of uncertainty. Yet, we still have to decide those uncertainties. For example, when COVID-19 hit the world during 2019-2022, we had to decide whether to take a vaccine. Given the statistical facts of several vaccines, how can we ensure that the vaccine is really effective or not? In this high-stakes situation, managing risk is really important because it involves our single and precious life.

That's where probability theory comes to mind. Probability theory is a science of uncertainty that we can quantify to help us make some decisions. Other situations or questions that may need a probability theory to answer include:
- Should we make an investment in this oil field?
- Should we lockdown the country to contain the spread of COVID-19?
- Should we build this new road?

That was in real life. How about in ML/AI specifically? Together with Linear Algebra and Calculus/Optimization, they play a crucial role. Many ML and AI approaches are based on probabilistic methods. For example:
- Classification/Regression: logistic regression, Bayesian classifier
- Clustering: gaussian mixture models, latent Dirichlet allocation
- Image Generation: variational autoencoder and diffusion models rely heavily on probabilistic models (let's discuss it in another post!)

## Random Experiment
Random experiment is the act of measuring a process **whose outcome is uncertain**. Below are examples of random experiments:
- Tossing a coin (when we toss a coin, we don't know whether it will land on head or tail)
- Throwing a die
- Drawing a colored ball from a basket
- Web browsing
- Phone usage
- Patient diagnosis

## Probability Model
Before we define the probability model, let's go deeper into what **Sample Space**, **Event**, and **Probability Measure** are.

### Sample Space \(S\)
Sample space is a set of all possible outcomes of an experiment. A sample space is discrete if it has a finite or countably infinite number of outcomes.

Finite (set) of outcome: throwing a dice -> $`S = {1,2,3,4,5,6}`$
Countably infinite: the set of all natural numbers (it is infinite, but we can count it)

### Event $`A`$
Event is a subset of the sample space - an event A is said to occur if the outcome of an experiment is a member of $`A`$. 

Example: Throwing a dice, got a number more than 5. Here, the sample space is $`{1,2,3,4,5,6}`$ and the event is $`{6}`$

### Probability Measure $`P`$
Probability measure $`P`$ on a sample space $S$ is a function defined on the subsets of S in such a way that:
- $`0 <= P(A) <= 1`$ , for all $`A \in S`$
- $`P(\emptyset) = 0`$ i.e. if $A$ is the empty set $`\emptyset`$, then $`P(A)=0`$. In other words, the probability of nothing happening is zero
- $`P(S) = 1`$ i.e. if $`A`$ is the entire sample space S, then $`P(A)=1`$
- $`P`$ is countably additive, i.e., if $`A_1, A_2, ...`$ is a finite or countable sequence of disjoint events (meaning that if a certain event happens, the other events can't happen), then $`P(A_1 \cup A_2 \cup ...) = P(A_1) + P(A_2) + ...`$

### Probability Model
After understanding the sample space, event, and probability measure, we can define probability model: A pair($`S,P`$) where $`P`$ is a probability measure on $`S`$