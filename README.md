# Review and implementation of the stochastic approximate proximal point method

* Park, Sungmin (@ppinsm)
* Lee, Yoonhyung (@yoonhyung93)
* Han, Seungji (@gkstmdwl9493)

### Introduction
Stochastic gradient descent method (SGD) is one of the most commonly used method for large-scale optimization problem. Despite of its wide use, SGD is highly sensitive to the choice of parameters such as initial step size and exhibits instability under finite iterations. There have been many attempts to alleviate this weakness of SGD, one of which is the stochastic proximal point method also known as the implicit stochastic gradient descent(P.Toulis and E.Airoldi, *Asymptotic and finite-sample properties of estimators based on stochastic gradients*. 2017). It has been shown that stochastic proximal point is stable and robust to various choice of initial step size. However, this method has limited application due to its model assumptions which is restricted to generalized linear models. Asi and Duchi (*Stochastic (approximate) proximal point methods: Convergence, optimality, and adaptivity*. 2019) gathered all models mentioned above and defined a unified class of models: stochastic approximate proximal point method (AProx method). They showed convergence and asymptotic normality of AProx iterates for convex objective functions. In addition, they proved that much of the results for convex objectives are still valid for weakly convex objectives as well. Our goal is first to verify theoretical results for convex functions by implementation. If results from the implementation of convex functions appear promising, we will expand our experiment to more general class of models, namely weakly convex functions.

### Project objective and schedule
* Review the following papers about stochastic approximate proximal point method :
  - Hilal Asi and John C. Duchi, Stochastic (Approximate) Proximal Point Methods: Convergence, Optimality, and Adaptivity. SIAM J.OPTIM. Vol. 29, No.3, pp. 2257-2290. (2019)
  - Hilal Asi and John C. Duchi, The importance of better models in stochastic optimization. Proceedings of the National Academy of Sciences (to appear). (2019)
  
* Reproduce and compare convergence behavior of methods in the the stochastic approximate proximal point class
  - Stochastic gradient descent method (SGD)
  - Stochastic proximal point method
  - Stochstic truncated gradient method
  - Bundle model
  
* Additional experiment on stochastic approximate proximal point method
  - Compare asymptotic covariance with empirical covariance of estimates
  - Check whether empirical distribution of estimates converges in distribution to normal distribution
  
* (Optional) Compare convergence behavior when hyperparameters of stochastic approximate proximal point method is changed
  - Step size
  - Batch size

...
