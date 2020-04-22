---
layout: default
landing: true
published: true
---

## Seminar
We organize a weekly seminar on machine learning. We discuss papers on ML, often (but not always) with connections to Earth science, climate and weather and materials science.

The seminar also allows members of the Hamburg machine learning community to connect and present their ongoing work. We meet in person at HZG, but we also welcome remote online participants and stream the meeting live on our [YouTube channel](https://www.youtube.com/channel/UCyXAYFO3h-tBIEbPEqMnNKw).

To get updates about each meeting or suggest a topic, please [join our mailing list](https://groups.google.com/forum/#!forum/mlhzg/join).

## Future Topics
### 5. TBA, 05.05.20

## Past Topics
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