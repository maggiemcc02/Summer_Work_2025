# Summer_Work_2025
In this repo, I collect the final set of notebooks for my work in the Summer of 2025.

This repo is the culmination of 5 research summers and one honours thesis. Some may say it is my scientific computing toddler. If you have any issues and/or questions, please get in contact with me, Maggie McCarthy :)


**Folder: Looping_Over_FixedAlpha_Tests**
- In these notebooks, I was experimenting with trying to find good fixed alpha values for the Hessian-based Mesh density function and for the Gradient-based Mesh Density function by looping over numerous choices for alpha.
- In all three notebooks, I employ continuation in alpha. In one notebook, I also do continuation in epsilon (alpha continuation loop inside the epsilon continuation loop)(Hessian M).

**Folder:  ManualMPvsFieldSplit_AlphaSolves_HessianRecovery_LinvsNonlinMeshSolves**
- As demonstrated in the name, this notebook collects a bunch of random, but potentially useful code bits.
- These codes explore the differences between the manual MP-Iteration and the FieldSplit MP-Iteration, solving for the alpha parameter for the Hessian-based M as described in (5.192) in HR, Hessian recovery for smoothing the Mesh Density function M, comparing linear and nonlinear mesh solves, and probably a lot more I have missed.

**Folder: alpha_scaledby_epsilon_tests**
- The notebooks in this folder comprise the work I did in the last week of work.
-  It is through the work in these notebooks that I experiment with, and learn that I should take, alpha = constant x epsilon^(-3/4) for the Hessian-based Mesh Density Function (5.192) with m=0 (minimizing L2 norm). I also learned that setting mesh_tol = 1e-8 results in oversolving in my MP-iteration. Rather, I swapped my mesh_tol to be mesh_tol = (1/10) x epsilon.
- I perform these experiments on the Linear Madden Problem and the Kopteva problem.
- These notebooks comprise my best results for the summer.

  Folder: FinalDefcon_EndofSummerWork
  - It is in this folder where I have a single notebook that I worked on on the last day of work.
  - In this notebook, I implement the work I did in 'Folder: alpha_scaledby_epsilon_tests' within a Defcon setting.
  - I did not get to finish this work. We think we need to work on the construction of the norm used in the deflation operator and maybe experiment with the power and shift parameters for the deflation operator.
 


  
