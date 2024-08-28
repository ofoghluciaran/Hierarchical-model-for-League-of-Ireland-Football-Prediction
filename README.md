# Bayesian Hierarchical Model for League of Ireland Football Prediction
This repository features a hierarchical model for predicting League of Ireland football outcomes using PyMC. The model adapts a 2010 approach by Baio and Blangiardo, originally designed for the Italian League, and incorporates Peadar Coyle's Six Nations Rugby model to infer each team's latent "strength." It uses Transfermarkt data from 2012-2023 to demonstrate probabilistic programming in football analytics.

# Objective
We aim to infer a latent parameter—the 'strength' of a team—using only their **scoring intensity**, with the available data being their scores and results. Accurately measuring a team's 'strength' directly is not feasible.

Probabilistic programming provides an excellent framework for modeling these **latent parameters**.

We aim to estimate the latent parameters—specifically, the strength of each team—that generate the observed data, namely the scorelines. Given that scorelines are an imperfect measure of team strength, our goal is to develop a model that quantifies the uncertainty around these underlying strengths.

In many cases, the exact Bayesian Model we require may not be explicitly defined, so we must approximate it. When a problem is too complex to solve directly, we employ approximation methods.

**Markov-Chain Monte Carlo** (MCMC) is used to draw samples from the posterior distribution. This versatile algorithm can be applied to nearly any model.
