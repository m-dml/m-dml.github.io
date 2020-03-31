---
layout: default
landing: true
published: true
---

## Research
Our ultimate aim is to understand and predict the complex dynamics of Earth’s atmosphere, ocean, land and ice.

### Physical Models
Numerical simulations based on known physics simulators handle complex systems well, but struggle with data assimilation, parameter tuning and uncertainty quantification.

<img align="left" src="L96.png" width="390" height="210" style="margin: 0px 20px 0px 0px"/> <span style="color:gray"><sub><sup>Simulation from the [Lorenz 96](http://eaps4.mit.edu/research/Lorenz/Predicability_a_Problem_2006.pdf) model. Defined as a system of differential equations, it exhibits many of the challenges appearing in more realistic models of climate and weather phenomena, such as chaotic dynamics and coupling of fast and slow processes.</sup></sub></span>

### Machine Learning
Conversely, machine learning techniques can absorb and process large datasets, but typically ignore physics and generalize poorly to new scenarios.

<img align="right" src="Unet.png" width="400" height="120" style="margin: 0px 0px 0px 20px"/> <span style="color:gray"><sub><sup>Example of a Unet architecture used for weather prediction, visualized using [NN-SVG](https://doi.org/10.21105/joss.00747).</sup></sub></span>

<br/><br/>

### The Combined Approach
We develop hybrid methods that combine deep learning with physical models in a Bayesian framework. Examples of this hybrid approach include:
* Neural networks that solve differential equations.
* Algorithms trained to infer model parameters using simulations.
* Machine learning models that respect physical laws.
* Flexible function approximators to fill gaps in our physical knowledge.
* Normalizing Flows, VAEs and GANs that model uncertainty in temperature, rainfall, fire and flooding.