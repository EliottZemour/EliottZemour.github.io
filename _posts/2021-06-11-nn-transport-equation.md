---
title: "Numerical Simulation of the Transport Equation with Neural Networks"
layout: post
date: 2021-06-11 22:10
tag: semester1
image: /assets/images/EPFL_Logo.png
headerImage: true
projects: true
hidden: true # don't count this post in blog pagination
description: ""
category: project
author: eliott
externalLink: false
---

This is a semester project carried out during my master studies in computational science and engineering at EPFL. 
* Duration: 5 months (February 2021 - June 2021)
* Supervisor: Prof. Marco Picasso (EPFL) 

---

<img class="image" src="/assets/images/semester1/motivational-example.png" alt="Alt Text">
<figcaption class="caption">Motivational example: coarse approximation and output of neural network for the solution of 2D transport problem.</figcaption>

---
### Abstract
In this report, we implemented numerical schemes for solving the one and two dimensional
transport problems. Numerical solutions are obtained with rather coarse grids and are passed
to a neural network which aims to improve the quality of such solutions by mapping them
into finer grids. We found strong performance as the networks implemented demonstrated the
capability to correct numerical diffusion artefacts and refine the solution at key points of the
grid. When the network is trained on a given type of functions, it appears to replicate very
well the targeted outputs. However, this approach does not seem to be very promising if the
goal is to train a model over basis functions, and use it for enhancing transported functions
that consist of linear combination of these.

---

### About this project
* Python code.
* Packages/Librairies: Keras, Tensorflow, Numpy.
* Colab notebooks available for reproducibility.

### Links
* Here's the link to the [report](/assets/projectreports/cse_project_report.pdf). 
* Link to the [repository](https://github.com/EliottZemour/NN-TransportEq-project).
* The dataset used in this project work is available on [Kaggle](https://www.kaggle.com/eliottzemour/neural-networks-for-tranport-equation).

