prj: project code  
Presentation: project paper  
Papers: papers of the analyzed optimizers  

# Analysis of some Variance Reduction Optimizers: SARAH, SpiderBoost and SNVRG

We proposed some *stochastic variance reduced gradient methods* for smooth non-convex optimization problems. All the analyzed algorithms represent, in many cases, valid alternatives to improve the performance of **Stochastic Gradient Descent**, by reducing its variance and therefore improving its convergence.

These considerations are observed also in empirical experiments. We have observed that all these algorithms in the non-convex case perform well, even *SARAH* which is originally used for convex functions problems. This result can be given from the particular structure of the loss function we are using to face the optimization problems: their shapes, in fact, show some convex areas for which SARAH is optimized. Another aspect that we can note from our analysis is the better functioning of *SNVRG* in presence of a large number of dimensions. However, we must keep in mind that *SNVRG* requires the use of many hyperparameters. We can instead say that *SpiderBoost* also works quite well, but that due to its sensitivity in the choice of S and Q and its performance almost on a par with *SARAH*, it cannot be considered a very good candidate.
