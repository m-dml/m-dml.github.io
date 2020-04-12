---
layout: default
landing: true
published: true
---

## Research
Our ultimate aim is to understand and predict the complex dynamics of the Earth’s atmosphere, ocean, land and ice.

### Physical Models
Numerical simulations based on known physics simulators handle complex systems well, but struggle with data assimilation, parameter tuning and uncertainty quantification.

<img align="left" src="L96eqs.png" width="288" height="81" style="margin: 0px 0px 0px 0px"/>
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
<span style="color:gray"><sub><sup>Parameter inference for the [Lorenz 96](http://eaps4.mit.edu/research/Lorenz/Predicability_a_Problem_2006.pdf) model, which it exhibits many of the challenges in models for climate and weather phenomena, such as chaotic dynamics and coupling of fast and slow processes.  </sup></sub></span>
<br/>
<img align="left" src="L96.png" width="360" height="260" style="margin: 0px 0px 0px 0px"/>
<img align="right" src="lorenz96_twoLevel_fig_schneider_5ss.png" width="260" height="260" style="margin: 0px 0px 0px 0px"/>
<br/><br/>

### Machine Learning
Conversely, machine learning techniques can absorb and process large datasets, but typically ignore physics and generalize poorly to new scenarios.

<img align="right" src="Unet.png" width="400" height="120" style="margin: 0px 0px 0px 20px"/> <span style="color:gray"><sub><sup>Example of a Unet architecture used for weather prediction, visualized using [NN-SVG](https://doi.org/10.21105/joss.00747).</sup></sub></span>

<br/><br/>

### Model-driven Machine Learning
We develop hybrid methods that combine the advantages of deep learning and physical modeling in a Bayesian framework. Examples of this hybrid approach include:
* Neural networks that solve differential equations.
* Algorithms that learn to infer model parameters using simulation results as training data.
* Machine learning models that respect physical laws.
* Flexible function approximators to fill gaps in our physical knowledge.
* Normalizing Flows, VAEs and GANs that model uncertainty in temperature, rainfall, fire and flooding.