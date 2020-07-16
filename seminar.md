---
layout: default
landing: true
published: true
---

## Seminar
We organize a biweekly seminar on machine learning, every second Tuesday at 3pm (GMT+2). We discuss papers on ML, often (but not always) with connections to Earth science, climate and weather and materials science.

The seminar also allows members of the Hamburg machine learning community to connect and present their ongoing work. We meet in person at HZG, but we also welcome remote online participants and stream the meeting live on our [YouTube channel](https://www.youtube.com/channel/UCyXAYFO3h-tBIEbPEqMnNKw).

To get updates about each meeting or suggest a topic, please [join our mailing list](https://groups.google.com/forum/#!forum/mlhzg/join).

## Future Topics

### 11. TBA 28.07.20

### 10. "Try to look like a little black cloud" 14.07.20

In light of recent meteorological events in Hamburg, the next ML@HZG seminar will focus on clouds.

We will begin with a well-written 3-page review[1] that discusses how cloud resolving models (CRMs) can play an important role in our understanding of our climate and its potential changes in the future, but impose immense computational demands.

We'll then discuss how small-scale CRMs can be used as cloud parameterizations for large-scale climate models, focusing on the Superparameterized Community Atmosphere Model (SPCAM) [2]. This approach aims to capture the two-way interactions between cloud physics and coarser-scale meteorological variables without paying the cost of a huge CRM simulation, but instead embedding a small CRM into each grid cell. Further work[3] showed how the embedded CRMs can be simplified without compromising accuracy.

Finally, we'll discuss how machine learning can be used to imitate the effect of the miniature CRMs used in SPCAM, which in turn aims to imitate what a large-scale CRM might look like. Recent work[4] has shown the neural networks can be trained reproduce the feedback between coarse-scale climate model variables and each grid cell's CRM, with a considerable reduction of computational.

As we'll discuss, often the true test of these techniques is their ability to match observed phenomena in large, long simulations!

Postscript: As discussed in the seminar, it's not totally clear why the MJO moves east, but there are some interesting theories as to why[5] (thanks to Eduardo Zorita for the reference).

[1] T. Schneider et al., “Climate goals and computing the future of clouds,” Nature Clim Change, vol. 7, no. 1, pp. 3–5, Jan. 2017, doi: 10.1038/nclimate3190.

[2] M. Khairoutdinov, D. Randall, and C. DeMott, “Simulations of the Atmospheric General Circulation Using a Cloud-Resolving Model as a Superparameterization of Physical Processes,” J. Atmos. Sci., vol. 62, no. 7, pp. 2136–2154, Jul. 2005, doi: 10.1175/JAS3453.1.

[3] M. S. Pritchard, C. S. Bretherton, and C. A. DeMott, “Restricting 32–128 km horizontal scales hardly affects the MJO in the Superparameterized Community Atmosphere Model v.3.0 but the number of cloud-resolving grid columns constrains vertical mixing,” Journal of Advances in Modeling Earth Systems, vol. 6, no. 3, pp. 723–739, 2014, doi: 10.1002/2014MS000340.

[4] S. Rasp, M. S. Pritchard, and P. Gentine, “Deep learning to represent subgrid processes in climate models,” PNAS, vol. 115, no. 39, pp. 9684–9689, Sep. 2018, doi: 10.1073/pnas.1810286115.

[5] B. Wang, F. Liu, and G. Chen, “A trio-interaction theory for Madden–Julian oscillation,” Geosci. Lett., vol. 3, no. 1, p. 34, Dec. 2016, doi: 10.1186/s40562-016-0066-z.


## Past Topics

### 9. "The Best of All Possible Worlds" 30.06.20
We consider the critically important and monstrously difficult problem of tuning climate model parameters to match observations (reviewed in [Hourdin et al., 2017](https://journals.ametsoc.org/bams/article/98/3/589/70022/The-Art-and-Science-of-Climate-Model-Tuning)). 

This process is quite challenging, because:
* Testing new parameter combinations through simulation incurs an immense computational cost.
* The aspects of the data we wish to match (warming trends, long-term means and variances) require long, global simulations.

We discuss several approaches to this problem:
* Gradient-based Optimization attempts to adjust model parameters by following the gradients, or derivatives of climate model outputs with respect to parameters. A major challenge for this approach is that we usually lack the ability to calculate or even approximate these derivatives. [Tett et al., 2017](https://gmd.copernicus.org/articles/10/3567/2017/gmd-10-3567-2017.pdf) get around this problem by using finite differencing, where derivatives are approximated using small perturbations to the parameters.
* History matching is a technique where nonlinear regression is used to learn an "emulator" or "metamodel" that maps directly between multiple tunable model parameters and real-world observables we'd like the original model to reproduce. Having estimated this parameter-observable relationship using a finite number of simulations, we can then identify all regions of parameter space for which the predicted model output is close to observations. [Williamson et al., 2013](https://link.springer.com/article/10.1007%2Fs00382-013-1896-4) and [Bellprat et al. 2012](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2012JD018262) use polynomial functions to build emulators for global and regional climate models resepctively. We also consider the more recent [Li et al., 2019](https://gmd.copernicus.org/articles/12/3017/2019/), which replaces the polynomial functions with simple neural networks.
* To demonstrate validation of a tuning scheme, [Bellprat et al. 2016](https://journals.ametsoc.org/jcli/article/29/2/819/35899/Objective-Calibration-of-Regional-Climate-Models) use history matching on regional climate models for two different regions, and compare the results.
<iframe width="560" height="315" src="https://www.youtube.com/embed/QQi3JRPiCcs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 8. "Uncharted History" 16.06.20
We discuss the paper "Artificial intelligence reconstructs missing climate information", Kadow et al. 2020, Nat. Geosci. [pdf](https://www.nature.com/articles/s41561-020-0582-5.epdf?sharing_token=QbCxMxkv1yFttqEFbh4FkNRgN0jAjWel9jnR3ZoTv0P2qUHXvupkkLyDpFacZ59nRBEIbALvzfpzSh-gBxsqgNpNQRCIHgzUmS4VsNCdAN8bOiDdHAMmDslOUvoPznb4U0cS2yHwzUSvv01Rym2EcDtqL9vDJL5U7CBAPd60mNM%3D) [code](https://github.com/FREVA-CLINT/climatereconstructionAI)

We are very happy to have the first-author of the paper with us to present the study!

The computer vision field of image inpainting [paper](https://dl.acm.org/doi/10.1145/344779.344972) uses several techniques to reconstruct broken images, paintings, etc. In recent years, more and more diverse machine learning techniques have boosted the field. A major step was taken by Liu et al. 2018 [paper](https://arxiv.org/abs/1804.07723) [video](https://www.youtube.com/watch?v=gg0F5JjKmhA&t=5s) in using partial convolutions in a CNN. The study shown here will transfer the technology to climate research. The presentation will show the journey of changing and applying the NVIDIA technique to one of the big obstacles in climate research: missing climate information of the past. Therefore a transfer learning approach is set up using climate model data. After evaluating test-suites, a reconstruction of [HadCRUT4](https://crudata.uea.ac.uk/cru/data/temperature/) - one of the most important climate data sets - is shown and analyzed.
<iframe width="560" height="315" src="https://www.youtube.com/embed/uzM5qPzpRQ8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 7. "Compressed Pressure", 02.06.20
The main paper for this session will be [Latent Space Physics: Towards Learning the Temporal Evolution of Fluid Flow](https://arxiv.org/pdf/1802.10123), Wiewel et al, 2019. Also see their [blog post](https://ge.in.tum.de/publications/latent-space-physics/).

We will also briefly discuss a [follow-up](https://ge.in.tum.de/publications/latent-space-subdivision/) from Wiewel et al. 2020, and a [related paper on generative fluid modelling](https://arxiv.org/abs/1806.02071) from the same group, Kim et al. 2019. The latter is nicely summarized in [this video](https://www.youtube.com/watch?v=hSDzOZ9IO8U).

For those interested in the underlying ML methods, this session will be about autoencoders and sequence-to-sequence models:

* [Autoencoders](https://www.jeremyjordan.me/autoencoders/) train pairs of neural networks for unsupervised learning of data representations, and Wiewel et al. use them to compress the high-dimensional volumetric fluid data.
* Sequence-to-sequence models allow to predict a variable-length output sequence from a variable-length input sequence, using a pair of recurrent neural networks. "seq2seq" [originated in natural language processing](https://arxiv.org/abs/1409.3215), but as we will see it can also be used to predict sequences of 3D images.
<iframe width="560" height="315" src="https://www.youtube.com/embed/gxpy24NYjd8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
<br/>
<br/>

### 6. "Minimalist Chaos", 19.05.20
We'll discus the Lorenz `96 model (L96) and its myriad uses. In ["Predictability - a problem partly solved"](http://eaps4.mit.edu/research/Lorenz/Predicability_a_Problem_2006.pdf), Edward Lorenz introduced a simple mathematical model exhibiting many of Earth science's core computational challenges.

Challenging features of L96 include chaotic dynamics, nonlinearity, combination of dissipative and conservative aspects and coupling of vastly differing scales in space and time. Chaos means that small perturbations in the model state due to numerical errors or observation noise will, over time, lead to large deviations in the future model state.

L96 is a frequent test case for algorithms tackling many fundamental problems. We consider two of these: parameter tuning, and parameterizing sub-grid processes:

* Marcel Nonnenmacher will describe work on identifying the 4 parameters of L96. This includes ["Recovering the parameters underlying the Lorenz-96 chaotic dynamics,"](https://arxiv.org/pdf/1906.06786.pdf) Mouatadid et al. 2019, ["Earth System Modeling 2.0"](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1002/2017GL076101), Schneider et al., 2017, as well as his own unpublished work.
* ["Coupled online learning as a way to tackle instabilities and biases in neural network parameterizations: general algorithms and Lorenz96 case study (v1.0)"](https://arxiv.org/pdf/1907.01351.pdf), Rasp 2020. This paper and a related [blog post](https://towardsdatascience.com/lorenz-96-is-too-easy-machine-learning-research-needs-a-more-realistic-toy-model-6add938f6cc0) discuss the design of parameterizations that approximate the effect of fast, fine-scale processes on slow, coarse scale ones. Linear and ML-based parameterizations are considered.
* Tobias Finn will guide us through stochastic parameterizations, which approximate deterministic chaos using randomness. ["Machine Learning for Stochastic Parameterization: Generative Adversarial Networks in the Lorenz '96 Model"](https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/2019MS001896), Gagne et al., 2020, uses Generative Adversarial Networks (GANs, see episode 5) to describe uncertainty in the tendency of coarse, slow variables as a result of unseen fast, fine variables. It builds on previous stochastic parameterizations without ML.

Finally, we'll revisit the original paper and the issue of predictability, nearly 25 years later.
<iframe width="560" height="315" src="https://www.youtube.com/embed/ckxIGFOu14Y" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 5. "Real Fake Clouds" 05.05.20
We discuss the paper "Modeling Cloud Reflectance Fields using Conditional Generative Adversarial Networks," Schmidt et al. 2020, arXiv.
[pdf](https://arxiv.org/pdf/2002.07579.pdf) [code](https://github.com/krisrs1128/clouds_dist)

This paper uses generative adversarial networks, or GANs. In the GAN framework, a generator network learns to generate "fake" data points while a second discriminator network learns to tell real from fake data. Schmidt et al. use GANs to predict cloud reflectance fields from meteorological variables such as temperature and wind speed. Given these meteorological variables, it can produce multiple realistic output patterns instead of an ensemble average. That is, the network attempts to learn the conditional probability distribution of reflectance given the input variables.

We start with a very brief introduction of GANs. More background can be found in Diego Gomez Mosquera's high accessible [blog post](https://medium.com/ai-society/gans-from-scratch-1-a-deep-introduction-with-code-in-pytorch-and-tensorflow-cb03cdcdba0f) or Ian Goodfellow's [extensive tutorial](https://arxiv.org/pdf/1701.00160.pdf).

Importantly, this paper wasn't able to get good results just by applying the GAN framework out of the box, and had to use some of the latest specialized tricks as well. So we'll briefly go through some of these tricks:

* Adding a term to the loss function that corresponds to supervised learning, as proposed for image to image translation tasks by Isola et al. 2018. [pdf](https://arxiv.org/pdf/1611.07004.pdf)
* Multi-scale discriminator and generator networks, via Wang et al. 2018. [pdf](https://arxiv.org/pdf/1711.11585.pdf)
* A least squares objective function, proposed by Mao et al. 2017 to avoid vanishing gradients. [pdf](https://arxiv.org/pdf/1611.04076.pdf)

Additional links from the discussion:
Variational Dropout and and the Local Reparameterization Trick [pdf](https://arxiv.org/pdf/1506.02557.pdf)
Dropout as a Bayesian Approximation: Representing Model Uncertainty in Deep Learning [pdf](https://arxiv.org/pdf/1506.02142.pdf)

<iframe width="560" height="315" src="https://www.youtube.com/embed/LZpHkkfN7qY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 4. "Far into the Future", 21.04.20
Lennard Schmidt from UFZ present on his work. He applies machine learning to do quality control for hydrological measurement data. He also uses a sophisticated convLSTM architecture to predict hydrological dynamics in an Elbe catchment basin. Code for a convLSTM layer in tensorflow/keras can be found [here](https://keras.io/examples/conv_lstm/).

Eduardo Zorita presents "Deep learning for multi-year ENSO forecasts," Ham et al. 2019, Nature. [link](https://www.nature.com/articles/s41586-019-1559-7)
This paper uses machine learning algorithms to predict the [El Niño/Southern Oscillation]((https://en.wikipedia.org/wiki/El_Ni%C3%B1o%E2%80%93Southern_Oscillation)) 1.5 years into the future, farther than previous methods have achieved. Notably, it trains on a combination of simulations and historical data.

Additional references on the predictability paradox in climate science:
"Do seasonal‐to‐decadal climate predictions underestimate the predictability of the real world?" Eade et al. 2014, Geophys. Research Letters. [link](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2014GL061146)

"Skilful predictions of the winter North Atlantic Oscillation one year ahead." Dunstone et al. 2016, Nature. [link](https://www.nature.com/articles/ngeo2824)

<iframe width="560" height="315" src="https://www.youtube.com/embed/vtOqMg48HlU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 3. "MetNet, Convolutional-Recurrent Nets, and the Self-Attention Principle" 07.04.20
Linda von Garderen presents on her work.

We cover Google Research's recent work on weather prediction: "MetNet: A Neural Weather Model for Precipitation Forecasting," Sønderby et al., 2020, arXiv.
[paper](https://arxiv.org/pdf/2003.12140.pdf), [blog post](https://ai.googleblog.com/2020/03/a-neural-weather-model-for-eight-hour.html)

To understand the ML tools that went into this work, we briefly review some concepts from earlier works:
* The convolutional LSTM, which combines convolutional and recurrent neural nets into a single architecture, as introduced by Xingjian et al. in 2015. [paper](http://papers.nips.cc/paper/5955-convolutional-lstm-network-a-machine-learning-approach-for-precipitation-nowcasting.pdf). [Review on LSTMs](Christopher Olah's reivew of LSTMs https://colah.github.io/about.html) by Christopher Olah. 
* Self-attention and the Transformer architecture, introduced by Vaswani et al. in 2017 https://arxiv.org/pdf/1706.03762.pdf, provide a new alternative to convolutional and recurrent nets. MetNet uses a specialized variant called Axial Attention (Ho et al., 2019)[paper](https://arxiv.org/pdf/1912.12180.pdf). We'll turn to a [blog post](http://www.peterbloem.nl/blog/transformers) by Peter Bloem for helpful illustrations. For further reading on the attention concept, see Lillian Weng's excellent [blog post](https://lilianweng.github.io/lil-log/2018/06/24/attention-attention.html#transformer)

With these concepts in mind, we examine how MetNet combines them, and consider their results from the perspectives of both ML and weather prediction.

Relevant discussion links:
* discussion between Stephan Rasp (TU Munich) and the MetNet authors on twitter. [link](https://twitter.com/raspstephan/status/1243139573980508160?s=20)
* F1 score used to quantify performance [link](https://en.wikipedia.org/wiki/F1_score)
* code on github for axial self-attention [link](https://github.com/google-research/google-research/blob/master/axial/transformers.py)

<iframe width="560" height="315" src="https://www.youtube.com/embed/2siOOD5p11U" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 2. "Don't Fear the Sphere" 31.03.20
We cover "[Spherical CNNs on Unstructured Grids](https://arxiv.org/pdf/1901.02039.pdf)," Jiang et al. 2019, ICLR. We also survey other ML approaches to spherical data (more links in the description on YouTube).
With 5 minute presentations by Julianna Carvalho, Tobias Finn and Lennart Marien.
<iframe width="560" height="315" src="https://www.youtube.com/embed/hwWeAd5_K20" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 1. "Hidden Fluid Mechanics" 24.03.20
We discuss the paper "[Hidden fluid mechanics: Learning velocity and pressure fields from flow visualizations](https://science.sciencemag.org/content/367/6481/1026)," Raissi et al. 2020, Science, and the more technical study from the same group, "[Physics Informed Neural Networks](https://www.sciencedirect.com/science/article/pii/S0021999118307125)," Raissi et al., 2019, J. Computational Physics.
Tobias Weigel from DKRZ explains the ML support team that forms part of the local Helmholtz AI unit.
<iframe width="560" height="315" src="https://www.youtube.com/embed/p-B0_gk8Uj4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>
