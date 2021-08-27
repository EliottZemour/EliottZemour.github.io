---
title: "Regularized Maximum Likelihood Estimation for Discrete Choice Models"
layout: post
date: 2020-12-17 22:10
tag: transpormle
image: /assets/images/EPFL_Logo.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: ""
category: project
author: eliott
externalLink: false
---

This is a project carried out for the CS-433 Machine Learning course at EPFL, in the framework of EPFL's [ML4Science](https://www.epfl.ch/labs/mlo/ml4science/) : Interdisciplinary Machine Learning Projects Across Campus.
* Supervisors ([EPFL TRANSP-OR lab](https://www.epfl.ch/labs/transp-or/)):
  * Nicola Ortelli
  * Michel Bierlaire

---

Discrete Choice Models (DCMs) aim to understand and model choices of individuals among a finite and discrete set of alternatives. Such models are mainly used by forecasters and policymakers to study consumer demand (e.g for transport mode choice). DCMs are based on Utility theory, which introduces the so-called utility functions designed to represent the preference structure of individuals among a given choice set.  
  
Specifications in DCMs are often introduced according to intuition, judgment and prior behavioral assumptions of the modeller. Therefore, utility specification represents a difficult task that one could see as a variable selection problem.
In this report, we investigate an automatized approach by introducing a regularization term in the likelihood function, aiming to push towards zero the parameters associated with the least relevant explanatory variables. Finally, the most penalized variables are discarded from the model with the expectation of not loosing too much information.  

---

### About this project
* Python code.
* Packages/Librairies: Biogeme and Pylogit (discrete choice models), scipy, numpy.
* Added the Box-Cox transformation to the pylogit package.


### Links
* Here's the link to the [report](/assets/projectreports/ml-project2_report.pdf). 
* Link to the [repository](https://github.com/EliottZemour/cs-433-project-2-lpmc_dcm).
* The dataset used is London Passenger Mode Choice (LPMC) revealed-preference data. A description of the features can be found [here](https://transp-or.epfl.ch/documents/technicalReports/CS_LPMC.pdf).
* Full details of the framework, dataset, and the models it was used to develop are given in [Hillel et al. (2018)](https://doi.org/10.1680/jsmic.17.00018).