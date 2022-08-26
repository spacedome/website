---
title: Projects
author: Julien
---

## Projects

----

### FEASTSolver.jl \[[code](https://github.com/spacedome/FEASTSolver.jl)\]
An implementation of the FEAST eigensolver and nonlinear extensions in Julia.

----

### FEASTconfig \[[code](https://github.com/spacedome/feast-config)\] \[[runnable webapp](/app/feastconfig/)\]
A javascript configuration tool for the advanced FEAST library features, prevents selection of invalid driver options. Made with Svelte. With compression the entire app is under 30KB!

----

### Quats.jl \[[code](https://github.com/spacedome/quats.jl)\]
A Quaternion library in Julia made for quaternion linear algebra.

----

### mandelbrot-rust (2016) \[[code](https://github.com/spacedome/mandelbrot-rust)\]
Simple Mandelbrot fractal rendering. Has smooth coloring and basic optimizations.

![fractal](/img/fractal-mandel-06.jpg)

----

### Learning Hyper-Parameters with Bayesian Optimization (2018) \[[pdf](/pdf/poster_CS682.pdf)\]
It is well known in the Machine Learning literature that a Grid Search for optimizing parameters is sub-optimal, and generally outperformed by a Random Search.
This project explored using Bayesian Optimization as a sequential search strategy, testing the method on the hyper-parameters of a relatively simple Neural Network performing image classification.

The main conclusion of this research is that incredible computational resources are needed to characterize NN hyper-parameter optimization methods, see the Google Vizier "paper" for context.
Despite this, Bayesian Optimization is a promising technique for sequential, potentially stochastic, optimization problems where the cost of sampling is a limiting factor.
For example, see my paper with Alex Dunn, *Rocketsled*, on applications of Bayesian Optimization to Computational Materials Science.

In a broader context, stop searching for parameters by hand, and consider random search over grid search if the relative importance of each parameter is unknown (for example some may not be important at all).
See the [paper](http://www.jmlr.org/papers/v13/bergstra12a.html) by Bergstra and Bengio for reference.
There is no reason to search parameters manually, there are many easy to use optimization codes to choose from, for example [skopt](https://scikit-optimize.github.io/).

----

### Cross-Validation Methodology in Materials Science (2018) \[[pdf](/pdf/poster_SULI.pdf)\]
Cross-validation is a critical part of statistical methodology, for ad hoc models cross-validation may be the only indication of model performance, and without a reasonable cross-validation methodology serious over-fitting can go undetected.
This issue is particularly relevant to domains where small data-sets with a comparatively large number of features is common, for example Materials Science or Genomics.
If the cross-validation method does not take into consideration the feature selection (that is, considering feature selection as part of model selection), a significant selection bias can occur, see [this paper](https://doi.org/10.1073/pnas.102102699) for an example with gene-expression data.
In general, a reasonably robust validation methodology should be chosen before model selection, and final hold-out sets should be used when possible.  
