---
layout: archive
title: ""
permalink: /tutorials/
author_profile: true
---

## Echo State Networks

<p align='center'>
<img src="../files/ESN_loop.png" style="width:600px">
</p>

Echo State Networks (ESNs) are a type of recurrent neural network, whose training consists in solving a linear system and does not require gradient descent [1,2]. ESNs have been shown to perform with similar accuracy to other reccurrent neural networks, such as LSTMs and GRUs [3]. 

Training ESNs is straightforward, but their performance is highly sensitive to the selection of hyperparameters.
In this [tutorial](https://github.com/aracca994/Echo-State-Networks) we provide an self-containted implementation of echo state networks with
 * an easy-to-follow and computationally efficient implementation of hyperparameter selection through Bayesian Optimization [4],
 * sparse matrix multiplication to improve computation efficiency and lower memory requirements.

We test the networks on the chaotic Lorenz system.  


## Computation of Lyapunov Spectrum and Kaplan-Yorke dimension

In chaotic systems, the dynamics are predictable only for finite times. This happens because infinitesimal errors in the prediction of the system increase in time with an average exponential rate given by the (positive) largest Lyapunov exponent of the system.

The dynamics of infinitesimal errors, namely tangent space dynamics, are defined by the entire set of Lyapunov exponents, the Lyapunov spectrum. Through the Lyapunov spectrum, the dimensionality of the solution, which is typically significantly smaller than the number of degrees of freedom can be estimated by the Kaplan-Yorke conjecture [5]. 

In this [tutorial](https://github.com/aracca994/Lyapunov-spectrum), we provide a Jacobian-free algorithm to compute the n largest Lyapunov exponents and the Kaplan-Yorke dimension of dynamical systems. 


# References 

- [1] H. Jaeger, [Scholarpedia](http://www.scholarpedia.org/w/index.php?title=Echo_state_network).

- [2] M. Lukoševičius, A Practical Guide to Applying Echo State Networks, pp. 659–686 (2012). Springer Berlin Heidelberg. 

- [3] P.R. Vlachas et al., Backpropagation algorithms and Reservoir Computing in Recurrent Neural Networks for the forecasting of complex spatiotemporal dynamics, Neural Networks (2020).

- [4] A. Racca & L. Magri, 2021 Robust Optimization and Validation of Echo State Networks for learning chaotic dynamics, Neural Networks (2021).

- [5] J. Kaplan & J. Yorke, Chaotic behavior of multidimensional difference equations, Lecture Notes in Mathematics (1979).
