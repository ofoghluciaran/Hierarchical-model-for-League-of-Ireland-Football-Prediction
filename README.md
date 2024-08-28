# Bayesian Hierarchical modelf for League of Ireland Football-Prediction
This repo features a hierarchical model for predicting League of Ireland outcomes using PyMC. It adapts a 2010 approach to simulate match results by Baio and Blangiardo based on Italian League scoring data and Peadar Coyle's approach to Six Nation's Rugby model, inferring each team's latent "strength." The model uses Transfermarkt data from 2012-2023, showcasing probabilistic programming for football analytics.







We want to estimate the latent parameters—specifically, the strength of each team—that generate the observed data, namely the scorelines.

Given that scorelines are an imperfect measure of team strength, our goal is to use a model that helps us quantify the uncertainty around these underlying strengths.

In many cases, the Bayesian Model we need may not be explicitly known, so we must approximate it.

If a problem proves too difficult to solve directly, we turn to approximation methods.

Markov-Chain Monte Carlo (MCMC) is a technique that samples from the posterior distribution.

Fortunately, this method is versatile and can be applied to nearly any model.














@incollection{citekey,
  author    = "<Peadar Coyle>",
  title     = "<Hierarchical model for Rugby prediction>",
  editor    = "PyMC Team",
  booktitle = "PyMC examples",
  doi       = "10.5281/zenodo.5654871"
}
