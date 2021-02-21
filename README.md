# Monte-Carlo-Simulation-with-Python

This article will describe how to use python with pandas and numpy to build a Monte Carlo simulation to predict the range of potential values for a sales compensation budget. This approach is meant to be simple enough that it can be used for other problems you might encounter but also powerful enough to provide insights that a basic “gut-feel” model can not provide on its own

## Problem Background

We will try to predict how much money we should budget for sales commissions for the next year. This problem is useful for modeling because we have a defined formula for calculating commissions and we likely have some experience with prior years’ commissions payments.

## Monte Carlo

Monte Carlo analysis might be a useful tool for predicting commissions expenses for the next year. At its simplest level, a Monte Carlo analysis (or simulation) involves running many scenarios with different random inputs and summarizing the distribution of the results.

Using the commissions analysis, we can continue the manual process we started above but run the program 100’s or even 1000’s of times and we will get a distribution of potential commission amounts. This distribution can inform the likelihood that the expense will be within a certain window. At the end of the day, this is a prediction so we will likely never predict it exactly. We can develop a more informed idea about the potential risk of under or over budgeting.

There are two components to running a Monte Carlo simulation:

the equation to evaluate
  - the random variables for the input
  - We have already described the equation above. Now we need to think about how to populate the random variables.

One simple approach would be to take a random number between 0% and 200% (representing our intuition about commissions rates). However, because we pay commissions every year, we understand our problem in a little more detail and can use that prior knowledge to build a more accurate model.

Let's buid the Monte Carlo simulation using python!!
