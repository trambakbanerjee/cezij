What is CEZIJ?
======
CEZIJ [1] is a novel framework for parameter estimation in joint models with multiple longitudinal outcomes along with a time-to-event analysis. Longitudinal data from modern datasets usually exhibit a large set of potential predictors and choosing the relevant set of predictors is highly desirable for various purposes including improved predictability. To achieve this goal, CEZIJ conducts simultaneous selection of fixed and random effects in high-dimensional penalized generalized linear mixed models and maintains the hierarchical congruity of the fixed and random effects, thus producing models with interpretable composite effects. It not only accommodates extreme zero-inflation in the responses in a joint model setting but also incorporates domain-specific, convex structural constraints on the model parameters. For analyzing such large-scale datasets, variable selection and estimation is conducted via a distributed computing based split-and-conquer approach [2] that massively increases scalability.

Installation
-----------
This repository holds the MATLAB toolbox `cezij.mltbx` that provides an implementation of the CEZIJ procedure developed in [1]. To install this toolbox, simply download `cezij.mltbx` in your computer and double click to install it. For a successful installation, please make sure that the following system requirements are met.

System Requirements
--------------
At a minimum your system must have access to 32GB RAM and at least 8 CPU cores for parallel computing. Additionally, the following software components are required. Please make sure that these are already installed before you attempt to install `cezij`.

1. MATLAB 2016b or higher with the following toolboxes (and their dependencies):

    a. Statistics toolbox
    
    b. Optimization toolbox
    
    c. Parallel Computing toolbox
    
    d. Data Acquisition toolbox

2. [CVX for MATLAB](http://cvxr.com/cvx/) (version 2.1 or higher)

Documentation
-----------
This repository includes a help file `cezij help.pdf` that explains how to use the toolbox with the aid of an example. To start using the toolbox, run `cezij_simulation.m` to reproduce the simulation experiment I in [1]. For using a different simulation setting or a different dataset altogether, please refer to `cezij help.pdf`.

References
----------
[1.] Banerjee, T., Mukherjee, G., Dutta, S., and Ghosh, P. (2019). A Large-scale Constrained Joint Modeling Approach For Predicting User Activity, Engagement And Churn With Application To Freemium Mobile Games. _(under review)_     

[2.] [Chen, X. and Xie, M.-g. (2014). A split-and-conquer approach for analysis of extraordinarily large data.
Statistica Sinica, pages 1655-1684.](http://www.stat.rutgers.edu/home/mxie/RCPapers/split_and_conquer_rev1_final.pdf)
