# Probabilistic Programming and Bayesian Computing with PyMC

Material for course on Bayesian Computation

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fonnesbeck/bayes_course_dec_2023/main) 

## Setup

This tutorial assumes that you have some form of [Anaconda](https://www.anaconda.com/products/individual#download-section) Python (with Python version 3.11) setup and installed on your system. If you do not, please download and install this on your system before proceeding with the setup. We recommend using the [Miniforge](https://github.com/conda-forge/miniforge#download) distribution of Anaconda, which is a lightweight version of Anaconda that is easier to work with.

The next step is to clone or download the tutorial materials in this repository. If you are familiar with Git, run the clone command:

    git clone https://github.com/fonnesbeck/bayes_course_dec_2023.git

otherwise you can [download a zip file](https://github.com/fonnesbeck/bayes_course_dec_2023/archive/main.zip) of its contents, and unzip it on your computer.
***
The repository for this tutorial contains a file called `environment.yml` that includes a list of all the packages used for the tutorial. If you run:

    mamba env create

from the main tutorial directory (if you installed Anaconda instead of Miniforge, use `conda` instead of `mamba`), it will create the environment for you and install all of the packages listed. This environment can be enabled using:

    mamba activate bayes_course  # Can also use "conda activate bayes_course"

Then, you can start **JupyterLab** to access the materials:

    jupyter lab

The binder link above should also provide a working environment.

## Pre-course Work

In advance of the course, we would like attendees to complete a short homework notebook that will ensure everyone has the requisite baseline knowledge. You can find this Jupyter notebook in the `/notebooks` subdirectory (under `Section0-Pre_Work.ipynb`). There is no need to hand this in to anyone, but please reach out if you have difficulty with any of the problems (or with setting up your computing environment) by creating an [issue](https://github.com/fonnesbeck/bayes_course_dec_2023/issues) in this repository, or by emailing.

## Course Outline

The course comprises twelve 75-minute modules of videoconference lectures, along with short associated hands-on projects to reinforce materials covered during lectures. The sections cover core materials related to Bayesian computation using PyMC, and include:

## Daily Schedule (All times are US Eastern)

- **10:00 to 11:15** First session
- **11:15 to 11:30** Break
- **11:30 to 12:45** Second session
- **12:45 to 13:00** Break
- **13:00 to 14:00** Third session

### Monday, December 4

**Introduction to Bayesian Models and PyMC** 
- The anatomy of a Bayesian model
- Probability density functions, inverse CDF sampling
- Bayesian comuptation and approximations
- The PyMC API
- PyTensor

**Markov chain Monte Carlo** 
- Rejection sampling
- MCMC basics
- Metropolis-Hastings samplers
- Gibbs samplers
- Problems with first-generation MCMC methods
- Using gradient information to improve MCMC
- Hamiltonian Monte Carlo
- NUTS
  
### Tuesday, December 5

**Hierarchical Models**
- Parital pooling
- Random effects
- Prediction

**Non-parametric Bayes** 
- Dirichlet processes
- Spline models
- Gaussian processes


### Wednesday, December 6

**PyMC Model Building and Model Checking** 
- Model building in PyMC
- Partial pooling
- Building hierarchical models
- Parameterizations
- Convergence diagnostics
- Goodness-of-fit checks
- Model comparison


### Thrusday, December 7

**The Bayesian Workflow** 
- Prior predictive checks
- Iterating models
- Posterior predictive checks
- Generative modeling
- Using the model