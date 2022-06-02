Machine Learning in Physics
===========================

These are the exercise notebooks for the Machine Learning class I taught
in Spring 2021.

These exercises were graded using JupyterHub and nbgrader.
Please email me if you are a lecturer and want to have the solutions.

A playlist with the [lecture videos] is  available.

Rationale
---------
The idea of this class is a little different from your usual shiny happy
pictures class on machine learning: there is a heavy focus on simple models,
in particular the linear model, and rigorous analysis.

There are three reasons for this:

 1. The linear model can be used to justify a lot of the "common wisdom" in
    machine learning rigorously and at same time pedagogically.  I found that
    actually being able to understand and prove, e.g., convergence behaviours
    is as important as observing it in-the-wild.
    
 2. From my experience, students approach a machine learning problem in physics from 
    "the wrong end", i.e., by throwing the most sophisticated model at it without
    much a-priori analysis instead of doing sophisticated a-priori analysis
    and then start with the simplest model that is reasonable.

 3. The convex cost functions means linear and logistic models are straight-forward
    to train.  I found writing simple training codes yourself greatly helps 
    "demystifying" machine learning libraries.


Structure
---------
The lecture can be roughly divided into three parts:

 1. **Python and Optimziation** (exercises 1–3):  Since physics undergrads at the TU Wien
    learn coding in C++ and not Python, the class starts with a Python crash course.  As exercises
    that go together with this intro and also are relevant to ML, we are looking at
    simple optimization problems and solve them with (accelerated) gradient descent or
    Newton's method.
    
 2. **Linear models** (exercises 4–7):  This is the centrepiece of the class.
    I am introducing the "scientific method for machines", i.e., the machine learning
    workflow, and we are going to run through it multiple times while cranking up
    the complexity.
    
    The core analysis technique used is the singular value decomposition.  We use it
    to prove the bias–variance tradeoff and perform convergence analysis for gradient
    descent.
    
 3. **Advanced models** (exercises 8–11):  Here we construct artificial neural networks
    by building them up from logistic models, which are introduced first.
    
    We then move to unsupervised learning, to make sure that students have seen another paradigm
    than supervised learning.  We can reuse our SVD analysis to construct low-rank approximations,
    which concludes the class.

Prerequisites
-------------
The class is geared towards advanced undergraduate students in physics.
They are supposed to have taken the following classes:

 1. Linear Algebra:  vector spaces, inner products, matrix products, 
    linear equations, vector and matrix norms, eigendecomposition
    
 2. Basic Coding (in C, C++ or Fortran): basic language constructs,
    loops, I/O, functions.  This is why the class starts with a Python
    crash course.

[lecture videos]: https://tube1.it.tuwien.ac.at/videos/watch/playlist/8b3e3cad-a55c-4ca5-a9bc-9f31dac7b585
