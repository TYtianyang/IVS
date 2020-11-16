![alt text](https://github.com/TYtianyang/IVS/tree/main/pic/ivs.png)

# Implied Volatility Surface with SC-BNN

The Python code for implied volatility surface project; Source of shape-constrained bayesian neural network.

## Introduction
This is a project lead by Prof. Dacheng Xiu in the Booth School of the University of Chicago. It aims to employ advanced machine learning techniques on the implied volatility surface problem in the field of financial engineering. Along the experiments of benchmark methods including splines, local kernel regression etc., we brought up a new method called shape-constrained bayesian neural network to address the challenge of bayesian inference in a constrained parameter space in neural network setting. 

## SC-BNN
The method considers the constrains by modifying the original prior distributions. It introduce the penalizing factor multiplying the original prior to represent how the model satisfy the constrains. In our work, we utilized an approximation function to the PDF of skewed normal to be the penalizing factor. On the base of that, we proceed on a simple yet efficient algorithm called "bayes-by-backprop" to do variational inference for the posterior. The method achieves comparable point prediction performance to the best of the benchmark methods, and satisfactory distributive prediction performance. Most importantly, the method empirically ensures all model samples satisfying the shape constrains.

## Contribution
1) The work gives a valid solution to the bayesian inference problem on the implied volatility surface.
2) The work brought up a general method that can serve as a benchmark in any machine learning bayesian inference problem with shape constrains.

