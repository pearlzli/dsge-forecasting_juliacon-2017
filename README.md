# Using Parallel Computing for Macroeconomic Forecasting at the Federal Reserve Bank of New York

Slides for a talk at [JuliaCon 2017](http://juliacon.org/2017/) on Wednesday,
June 21st at 1:30 pm.

## Abstract

This talk will give an overview of how researchers at the Federal Reserve Bank
of New York have implemented economic forecasting and other post-estimation
analyses of dynamic stochastic general equilibrium (DSGE) models using Julia’s
parallel computing framework.

This is part of the most recent release of
our [DSGE.jl](https://github.com/FRBNY-DSGE/DSGE.jl) package, following our
ports of the DSGE model solution and estimation steps from MATLAB that were
presented at JuliaCon in 2016. I will discuss the technical challenges and
constraints we faced in our production environment and how we used Julia’s
parallel computing tools to substantially reduce both the time and memory usage
required to forecast our models. I will present our experiences with the
different means of parallel computing offered in Julia - including an extended
attempt at using DistributedArrays.jl - and discuss what we have learned about
parallelization, both in Julia and in general.

In addition, I will provide some of our new perspectives on using Julia in a
production setting at an academic and policy institution. DSGE models are
sometimes called the workhorses of modern macroeconomics, applying insights from
microeconomics to inform our understanding of the economy as a whole. They are
used to forecast economic variables, investigate counterfactual scenarios, and
understand the impact of monetary policy. The New York Fed’s DSGE model is a
large-scale model of the U.S. economy, which incorporates the zero lower bound,
price/wage stickiness, financial frictions, and other realistic features of the
economy. Solving, estimating, and forecasting it presents a series of
high-dimensional problems which are well suited for implementation in Julia.

## Disclaimer

This talk reflects the experience of the author and does not represent an
endorsement by the Federal Reserve Bank of New York or the Federal Reserve
System of any particular product or service. The views expressed in this talk
are those of the authors and do not necessarily reflect the position of the
Federal Reserve Bank of New York or the Federal Reserve System. Any errors or
omissions are the responsibility of the authors.
