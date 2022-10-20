---
layout: default
landing: true
published: true
---

## Seminar
We organize a biweekly seminar on machine learning, every second Tuesday at 3pm (GMT+2). We discuss papers on ML, often (but not always) with connections to Earth science, climate and weather and materials science.

The seminar also allows members of the Hamburg machine learning community to connect and present their ongoing work. We meet in person at Hereon, but we also welcome remote online participants and stream the meeting live on our [YouTube channel](https://www.youtube.com/channel/UCyXAYFO3h-tBIEbPEqMnNKw).

To get updates about each meeting or suggest a topic, please [join our mailing list](https://groups.google.com/forum/#!forum/mlhzg/join).

## Future Topics


**For 2022 we are continuing our seminar on Zoom only (not on YouTube)**. We're hoping to encourage more discussion and exchange of ideas in this format, but we are always accepting new subscriptions to our mailing list if you'd like to join. Participants from all research fields and institutions are welcome!

TBA

## Past Topics

### 53. "A world wide web for spatial interpolation" 25.10.2022

On Tuesday, October 25 at 3pm, our ML Seminar will cover "Positional Encoder Graph Neural Networks for Geographic Data," by K. Klemmer, N. Safir, and D. B. Neill.[1]
 
we will look at PE-GNN, a framework based on Graph neural networks that provide an improved performance on geographical data interpolation and regression. PE-GNN includes a positional encoder that learns spatial context embeddings for each point coordinate that improves predictions. The authors claim that this is the first GNN-based approach that is competitive with Gaussian processes on spatial interpolation tasks.

[1] K. Klemmer, N. Safir, D. B. Neill. ["Positional Encoder Graph Neural Networks for Geographic Data"](https://arxiv.org/abs/2111.10144)



### 52. "Nvidia killed the NWP (clu)stars" 11.10.2022

On Tuesday, October 11 at 3pm, our ML Seminar will cover "FourCastNet: Accelerating Global High-Resolution Weather Forecasting using Adaptive Fourier Neural Operators," by T. Kurth, S. Subramanian, P. Harrington, J. Pathak, M. Mardani, D. Hall, A. Miele, K. Kashinath, A. Anandkumar.[1]
 
we will discuss FourCastNet, a new solution to a global weather emulator using ML [1]. The authors implemented Adaptive Fourier Neural Operators to solve the dimensionality problem and scaled their approach to ~10,000 GPUs. This results in a surrogate weather model with a 1 km resolution that only takes 6 hours to train. Inference can even be done on a single GPU-node with a speedup to 80,000 times compared to traditional NWPs. 


[1] T. Kurth, S. Subramanian, P. Harrington, J. Pathak, M. Mardani, D. Hall, A. Miele, K. Kashinath, A. Anandkumar. ["FourCastNet: Accelerating Global High-Resolution Weather Forecasting using Adaptive Fourier Neural Operators"](https://arxiv.org/abs/2208.05419)


### 51. "Good neighbours make good parametrizations" 27.09.2022

On Tuesday, September 27 at 3pm, our ML Seminar will cover "Non-local parameterization of atmospheric subgrid processes with neural networks," by Wang, Yuval & O'Gorman.[1]
 
Both classical an ML-based parameterization attempt to model sub-grid-scale processes based on the coarse-grained atmospheric or ocean variables present at each grid cell or grid column. This paper goes beyond this standard practice, asking "what if we use information from neighboring grid columns too?" Using this approach, they attempt to predict the tendency of precipitating water due to cloud microphysics in coarse-grained aquaplanet simulations.


[1] Wang, Peidong, Janni Yuval, and Paul A. O'Gorman. ["Non-local parameterization of atmospheric subgrid processes with neural networks." Journal of Advances in Modeling Earth Systems](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2022MS002984)

### 50. "Run, Chemistry, Run!" 13.09.2022
On Tuesday September 13 at 3pm, ML Seminar comes back from a summer break. We are going to discuss a recent paper by Makoto M. Kelp et al "An Online-Learned Neural Network Chemical Solver for Stable Long-Term Global Simulations of Atmospheric Chemistry" [1]. The discussion is going to be led by our new postdoc Dr. Andrey Vlasenko.
 
In this paper, the authors train an ML solver for GEOS-chem model to solve coupled kinetic equations describing the chemical mechanism. A solver implemented with an autoencoder trained online outperforms an implicit Rosenbrock solver. Another interesting aspect of this implementation is the dramatic increase in the stability of simulations. However, appearance of pattern biases stands as a limitation for using this solver.

[1]  Kelp, Makoto M., Daniel J. Jacob, Haipeng Lin, and Melissa P. Sulprizio. [“An Online-Learned Neural Network Chemical Solver for Stable Long-Term Global Simulations of Atmospheric Chemistry.”](https://doi.org/10.1029/2021MS002926)

### 49 . "Recovering Ancient History" 12.07.2022
On Tuesday July 12 at 3pm, Siddhant Agarwal from DLR will present his publication "Deep learning for surrogate modeling of two-dimensional mantle convection". [1]

So far in our machine learning seminars, we have discussed problems where ML has played an important role in short-term or seasonal forecasting. In the paper for the seminar, we now learn about a problem at a very different timescale that involves simulating models of the planet's mantle over timescales of thousands of years. Due to sparse observations, the initialization of model parameters becomes a rather tedious process. While simplified estimations using 1D models have been useful, 2D models contain more information but can be much slower.
In this paper, the authors use feed-forward neural networks and LSTMs to develop reliable surrogates for simulating 2D mantle convection. These are capable of estimating the temperature fields to a high degree of accuracy. We will discuss the challenges of the problem, data used and the implications of this work. 

[1]  Agarwal, S., Tosi, N., Kessel, P., Breuer, D., & Montavon, G. (2021, November 4). [Deep learning for surrogate modeling of two-dimensional mantle convection. Physical Review Fluids.](https://elib.dlr.de/146282/1/PhysRevFluids.6.113801.pdf)


### 48. "Not your Usual Parameterization" 31.05.2022
For our next seminar on May 31 at 3pm, we will discuss the paper "Deep Learning Based Cloud Cover Parameterization
for ICON" [1]. We are happy to announce that the first author, Arthur Grundner from DLR, will present the paper.

In many previous seminars we have discussed papers where the authors have applied machine learning in order to solve the problem of parameterization in weather and climate models. Although we have covered studies spanning convection to gravity wave drag parameterization, often these are limited to simpler model scenarios such as aquaplanets.

In the paper for the seminar, the authors tackle the problem of cloud cover parameterization using ICON SRM (storm-resolving model). This is the first time we'll discuss a paper where machine learning has been applied in ICON. The authors train neural networks to learn cloud cover variables using atmospheric state variables. We will discuss the experimental setup, the generalization ability of the networks, the interpretability of the ML model and the implications of this work. 

[1] Grundner, A., Beucler, T., Gentine, P., Iglesias-Suarez, F., Giorgetta, M. and Eyring, V., 2022. [Deep Learning Based Cloud Cover Parameterization for ICON.](https://arxiv.org/abs/2112.11317)


### 47. "They are the same picture" 17.05.2022

After having now had a lot of very specialized ideas and applications for ML in the earth system sciences in recent episodes, we would like for the next ML Seminar to take a step back and have again a look at the broader picture. For this, we will go through the challenges of ML in climate and weather applications and their differences described in [1]. We are looking forward to a lively discussion on where you think the broader challenges lie and maybe how to overcome them.

[1] Watson-Parris, Duncan. ["Machine learning for weather and climate are worlds apart."](https://arxiv.org/abs/2008.10679) Philosophical Transactions of the Royal Society A 379.2194 (2021): 20200098.


### 46. "Mapping to the Windows" 03.05.2022
On Tuesday, May 3 at 3pm Julianna Carvalho-Oliveira will discuss her latest publication "Self-Organizing Maps Identify Windows of Opportunity for Seasonal European Summer Predictions".[1]

Seasonal predictability of weather systems has always been a challenge. It is generally associated with planetary scale dynamical weather patterns. In case of Europe, seasonal predictability of summer climate is closely linked to the leading modes of atmospheric teleconnections associated with the North Atlantic jet stream. But current state-of-the-art models suffer from heavy biases and uncertainty when it comes to predicting the behavior of the jet stream.

In this paper, the authors attempt to identify atmospheric conditions that favor more predictable states of the atmosphere. For this, they combine an ensemble seasonal prediction system with a neural network-based classifier involving Self-Organizing Maps. This method helps to identify initial atmospheric conditions that correspond to a high predictability of the dominant modes of variability in the North Atlantic jet stream. 

We will discuss the theoretical aspect of the problem, the reasons for choosing self-organizing maps and the implications of the work. 

[1] Carvalho-Oliveira, J., Borchert, L. F., Zorita, E., & Baehr, J. (2022). [Self-organizing maps identify windows of opportunity for seasonal European Summer Predictions.](https://www.frontiersin.org/articles/10.3389/fclim.2022.844634/full)


### 45: "Data-driven discovery of Governing Equations" 19.04.2022

On Tuesday, April 19 at 3 pm we will discuss the paper "Data-driven discovery of coordinates and governing equations".[1]

In recent years, the field of data-driven discovery of governing equations has garnered a lot of attention as it has the potential to transform data-rich fields that lack well-characterized quantitative descriptions.
Previous approaches using sparse regression methods rely on an effective coordinate system in which dynamics have a simple representation. In this paper, the authors combine a custom deep autoencoder network with sparse identification of nonlinear dynamics (SINDy) to develop a new data-driven method for discovering interpretable, low-dimensional dynamical models and their associated coordinates from high-dimensional data. This approach is successfully applied for the the canonical chaotic Lorenz system, a 2D reaction–diffusion system, and a 2D spatial representation of the nonlinear pendulum.

[1] S. Champion, B. Lusch, J. N. Kutz, L. Brunton, [Data-driven discovery of coordinates and governing equations](https://www.pnas.org/doi/10.1073/pnas.1906995116).

### 44: "Machine masters Math?" 05.04.2022

On Tuesday, April 5 at 3pm we will discuss the paper "Grokking: Generalization Beyond Overfitting on Small Algorithmic Datasets". [1]

In this paper, the authors discuss a strange phenomena they encountered while overfitting an ML model. They observe that a model near convergence, but with low generalization capability, on continual training managed to reach a point where it was able to provide close to a 100% accuracy on validation dataset. The dataset used is made up of binary operations including addition and subtraction. This sudden jump in the ability to generalize to new datasets is worth deconstructing.

The authors call this phenomenon "grokking", referring to what seems like the ability of the model to somehow understand the underlying patterns within the dataset, which perhaps raises the question if this network had indeed learnt the intuition behind mathematical operations. In the seminar, we will discuss the special datasets they train on, the models used and the various hyperparameters that affect this phenomenon. We will also discuss perhaps why this phenomena has remained under the radar so far and what are its consequences. 

[1] Power, A., Burda, Y., Edwards, H., Babuschkin, I., & Misra, V. (2022, January 6). [Grokking: Generalization beyond overfitting on small algorithmic datasets](https://arxiv.org/abs/2201.02177).


### 43: "Learning to Assimilate" 22.03.2022

This seminar we are going to discuss a paper that applies deep learning to data assimilation in a new way. Data Assimilation is the problem of searching for an initial condition for which a model accurately predicts observed data, and is a central task for weather forecasting. 

In this paper, a convolutional neural network was used to learn an inverse observation operator (a mapping function between observations and physics-based space) [1]. Then this operator can be used to map observations trajectory into physical trajectory to use the first state as an initial state for data assimilation optimisation problem. Alternatively, they present a hybrid optimisation method when two optimisation problems are solving sequentially: first minimising objective function in physical space and then minimising in observational space. The results for a single-level Lorenz96 model and a two-dimensional turbulent fluid model show forecast quality increase. 

[1] Thomas Frerix, Dmitrii Kochkov, Jamie A. Smith, Daniel Cremers, Michael P. Brenner, Stephan Hoyer. [Variational Data Assimilation with a Learned Inverse Observation Operator](https://arxiv.org/abs/2102.11192). 



### 42: "Paint-by-numbers - Connect the little dots to forecast weather" 08.03.2022

In previous episodes, we have visited the weather-bench dataset and seen multiple approaches on solving the global weather prediction task. In the next seminar, we will for the first time discuss an article, where the author tackled the challenge using a graph neural network [1]. Therefore, we will give a brief introduction on graph representations and graph neural networks, to understand parts of the very clever bits and pieces the author combined to one framework. The resulting neural network trained on reanalysis data [2] was tested on hindcasts, where the author claims it not only is as good as state of the art NWPs (GFS and ECMWF), but in certain cases even outperforms them.

[1] R. Keisler, [Forecasting Global Weather with Graph Neural Networks](http://arxiv.org/abs/2202.07575), arXiv:2202.07575 [physics], Feb. 2022.

[2] S. Rasp, P. D. Dueben, S. Scher, J. A. Weyn, S. Mouatadid, and N. Thuerey, [WeatherBench: A benchmark dataset for data-driven weather forecasting](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020MS002203), J. Adv. Model. Earth Syst., vol. 12, no. 11, Nov. 2020. 
<br/>
<br/>

### 41: "Futureproof Your Training Data" 22.02.2022

On Tuesday, Feb. 22 at 3pm we will discuss the paper "Climate-Invariant Machine Learning".[1] This paper comes highly recommended for its interesting concepts, clear presentation and "dream team" of prominent authors at the intersection of climate and ML.

It addresses the poor capability of neural networks to generalize to new training data, using physics-inspired nonlinear transformations of the input variables that reduce the mismatch between training and testing scenarios. They apply this approach to sub-grid-scale parameterization learning in 3 climate models, and show that these data transformations allow the models to generalize to new climates and even model geographies.

While it's not uncommon for ML practitioners to try several possible representations of input data, this paper takes a principled approach to deriving the best data transformation based on specialized domain knowledge. Applying techniques for ML model interpretation, they uncover the surprising result that transforming the input data causes their NNs to learn mostly local dependencies that generalize better than other non-causal correlations in the input variables. Thus, the authors were able to achieve a result similar to the inductive biases provided by convnets, but do so instead by transforming inputs to a fully connected net.

[1] Beucler T, Pritchard M, Yuval J, Gupta A, Peng L, Rasp S, Ahmed F, O'Gorman PA, Neelin JD, Lutsko NJ, Gentine P. Climate-Invariant Machine Learning. arXiv preprint arXiv:2112.08440. 2021 Dec 14. [pdf](https://arxiv.org/pdf/2112.08440.pdf)
<br/>
<br/>

###  40: "Foiled Again?" 08.02.2022

On Tuesday February 8, 2022 at 3pm we will discuss the paper [Towards high-accuracy deep learning inference of compressible turbulent flows over aerofoils](https://arxiv.org/abs/2109.02183).

In past seminars we have covered the topic of using machine learning methods for learning fluid dynamics, be it from equations (seminar 1 and 25) or data generated from solving equations (seminar 11). The paper for this seminar builds upon ideas discussed in Seminar 7 where the authors tried to learn physics based representations for capturing the temporal evolution of fluid flow.  In this paper, the authors present a deep learning approach to infer the Reynold's averaged Navier-Stokes solutions for flow in compressible fluids. 

 
The deep neural network model used is based on a U-net which is used for encoding the geometric information and for decoding the subsequent flow fields. The authors compare the solutions provided by the machine learning algorithm to those produced by a Computational Fluid Dynamics model and note the significant speed up provided by the use of the neural network. 

We will discuss the structure of the model used, the challenges of the problem being solved and the limitations and further applications of this method. 
<br/>
<br/>

### 39: "Extreme Events, Modest Models" 25.01.2022

On Tuesday, January 25 at 3pm, we will discuss the paper, [Using Machine Learning to Analyze Physical Causes of Climate Change: A Case Study of U.S. Midwest Extreme Precipitation](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021GL093787).

In this paper, the authors tackle the task of defining, predicting and understanding extreme precipitation events in the US midwest. The authors start by defining a threshold for extreme precipitation events using historical station-based data and then develop a machine learning model to successfully classify precipitation events as "extreme events" based on atmospheric conditions.

This is followed by an interpretation study of the CNN used for classification, where the main goal is to investigate the relationship between atmospheric conditions and extreme precipitation events so as to answer the questions about the frequency and intensity of extreme events in a changing climate. We will go through the problem statement, methodology and the relevant results from the study during the seminar and discuss if these methods have the potential to perhaps disentangle complex interactions in the atmosphere.
<br/>
<br/>

### 38: "A Surge of Ensembles" 11.01.2022


We kickstart the machine learning seminars for 2022 on Tuesday, January 11 at 3pm. Dr Eduardo Zorita will lead the discussion on the paper, [Exploring deep learning capabilities for surge predictions in coastal areas](https://www.nature.com/articles/s41598-021-96674-0).

In this paper, the authors tackle the critical task of predicting the surge component of sea level variability from atmospheric conditions by making use of reanalysis data and observations from tide stations. They use various machine learning architectures including CNNs and LSTMs for generating ensemble based forecasts and compare the results to a global tide model.

After analyzing the results from over 736 stations distributed worldwide, the authors point to some interesting observations regarding the predicting capacity of the machine learning models. Similarly, seasonal variations are also analyzed in the paper. We will cover these interesting findings along with the general methodology applied in the paper.
<br/>
<br/> 

### 37. "What kind of a Storm are you?" 30.11.2021

Classification of convective storms depending on their severity has become more challenging in a changing climate. The major problem of machine learning-based methods for classification is their weak generalization capabilities to unseen scenarios which may result from changes in mean climatological temperature and moisture level. In the paper, [A benchmark to test generalization capabilities of deep learning methods to classify severe convective storms in a changing climate](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020EA001490), the authors develop a convolutional neural network-based classifier for classifying convective storms that are generated from models under the current climatic conditions. They then test the generalization capabilities of the model by evaluating its performance in classifying storms that are generated on a warmer Earth. 

 To further make sense of the physical relationships learned by the neural network, the authors use interpretation methods such as feature importance and saliency maps.  

 On Tuesday the 30th November at 3:00 pm, we would like to discuss this paper with you. We will go into the details of the framework of the problem, methodology, generalization capabilities of this method, and interpretation methods used to understand the underlying physical relationships. 

<br/>
<br/> 
### 36. "One column, many steps" 16.11.2021

On Tuesday Nov. 16 at 3:30 pm (note the later time!), we'll discuss [Prognostic Validation of a Neural Network Unified Physics Parameterization.](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018GL078510) This paper aims to train an ML model to reproduce moisture and temperature trends in a coarse resolution CAM atmospheric model, by training on data from a high-resolution CAM model.

 Supervised training on single-time-step updates can reach very high accuracy, but still result in inaccuracy or instability over many time steps. To address this, the paper proposes running the ML parameterization over multiple time steps during training to provide better feedback to the training procedure. They show that this can improve accuracy without changing the neural network at all.

 This approach faces the technical challenge that results over multiple time steps would involve the CAM dynamical core, which is fundamentally incompatible with the numerical optimization used to train neural networks. To get around this, the paper uses the idea of single column modelling from classical parameterization tuning in Earth science: the parameterization is trained for individual columns, with the advective forcing from neighboring columns "frozen" during training. We'll discuss this approach, its results and consider advantages and disadvantages.

<br/>
<br/>
### 35. "A Rare Case of Medium Range Weather Forecasting Well Done with Resnets" 02.11.2021

On the 2nd February 2020 Rasp and Thurey published an article introducing their medium range forecasting benchmark dataset "WeatherBench". Exactly one year later, on the 2nd February 2021 they released the Paper [Data-Driven Medium-Range Weather Prediction With a Resnet Pretrained on Climate Simulations: A New Model for WeatherBench](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020MS002405), where they set new baseline results for the previously mentioned dataset.
 
On Tuesday the 2nd November at 3:00 pm, we would like to discuss these new baselines with you.
<br/>
<br/>

### 34. "A Bin-full of Clouds" 19.10.2021

Cloud microphysics parametrizations tend to be simplified and often the complex parametrization schemes lead to a significant slowdown in weather prediction models. In Episode 22 we discussed warm rain emulation from a droplet based scheme. Between the extreme computational costs of droplet based schemes and simplification of bulk moments, there exist bin-based parametrization schemes which represent cloud and rain droplets as a distribution. In the paper for the seminar, [Machine Learning the Warm Rain Process](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020MS002268), the machine learning model (comprising of multiple neural networks) learns one such bin-based scheme.


We will go over the details of the spectral bin parametrization scheme used and why it can cause a 400% slowdown when used in a GCM. We will discuss how the ML based parametrization provides a huge speedup, its general performance when coupled with the GCM and the implications of these results for future research.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4u4KuhOO9MU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br/>
<br/>


### 33. "The Big Gravity Wave Drag Race" 05.10.2021

The biggest uncertainties in numerical weather predictions (NWPs) still arise from parameterizations. Even though 
simulators exist, which are better than the parameterizations implemented in the NWPs, they cannot be used due to higher 
computational costs. Therefore, we are excited to announce our guest speaker Matthew Chantry from the European Centre 
for Medium Range Weather Forecasts, who investigated the use of neural networks to emulate gravity wave drag 
parameterizations [(Chantry et al.)](https://doi.org/10.1029/2021MS002477). 
By training a NN on a higher complexity version of the parameterization and plugging it back into 
a NWP, they were able to produce more accurate forecasts than in the existing scheme by keeping the computational cost 
of the complete NWP the same.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_wm1dEIO-xU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>



### 32. "You know, I am something of a classifier myself" 07.09.2021

Labelled data is hard to come by, usually requiring an expert to sit down and look at thousands of examples. Generating / collecting data on the other hand becomes easier every day. So we are now in a position where we theoretically have enough data to train huge networks, but not enough labels to practically do that in many cases. 
The approach we will be talking about in the next seminar addresses this issue [(Chen et al.)](https://arxiv.org/abs/2002.05709). The idea is to compare training samples only to themselves without any labels in a pretraining step and only afterwards use a few labelled examples to fine-tune the neural network. They were able to get the same accuracy on the ImageNet benchmark dataset as supervised state of the art methods, but using only 1% of the labelled data.
We will also have a look at how this method can be used in an Earth-System-Science example to detect irrigation from satellite images. [(Agastya et al.)](https://arxiv.org/abs/2108.05484) 

<iframe width="560" height="315" src="https://www.youtube.com/embed/xwYMSTOfE-I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 31. "Enchanting the Chemical Forest" 24.08.2021

On Tuesday, August 24 at 3 PM (GMT+2), we'll discuss two papers applying machine learning to atmospheric chemistry. Coupling realistic chemical calculations to an atmospheric model imposes extreme computational costs, both for long-term climate modelling and short-term air quality forecasts. These studies attempt to reduce these costs by learning an inexpensive proxy for the chemical processes. [Keller et al.](https://gmd.copernicus.org/articles/12/1209/2019/gmd-12-1209-2019.pdf) use random forests for this, while [Kelp et al.](https://arxiv.org/ftp/arxiv/papers/1808/1808.03874.pdf) use deep neural networks.

We'll briefly review the nature of the chemical processes being modelled, and the basics of random forests as covered in previous episodes (19 and 21), and discuss the advantages, limitations and results of these two studies.

<iframe width="560" height="315" src="https://www.youtube.com/embed/rbRtVaUOeGQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 30. "Looking into the Black Box" 13.07.2021

On Tuesday, July 13 at 3 PM (GMT+2) we discuss the paper [Physically Interpretable Neural Networks for the Geosciences: Applications to Earth System Variability](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019MS002002). In most applications of machine learning within the Geosciences the main goal of the research is to generate accurate results. Often in these cases, the underlying ML can appear quite opaque. The main goal in the paper for the seminar is to use interpretation techniques in order to gain a deeper scientific understanding of what the neural network learns.

In this study, the neural networks are tasked with predicting scientifically well-studied phenomena such as occurrence of El-Nino and seasonal sea surface temperature variability. The authors focus on using backward optimization and layerwise relevance propagation (LRP) methods that aim to decipher how every input field affects the neural network output. Not only do these help in understanding the neural network but more importantly, as the authors show, these interpretations can themselves be used to advance our understanding of the Earth System. In [Making the Black Box More Transparent: Understanding the Physical Implications of Machine Learning](https://journals.ametsoc.org/view/journals/bams/100/11/bams-d-18-0195.1.xml) further applications of interpretation methods can be found.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/VvcUceL3U5I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 29. "Why does it always rain on me?" 15.06.2021 
Caroline Arnold from DKRZ will present recent developments in using ML for precipitation nowcasting. High-resolution precipitation nowcasting, with a lead time of up to two hours is relevant for many weather-dependent real world decisions such as those concerning commercial aviation, power utilities, and transportation services. Accurate nowcasts can provide a timely warning for extreme flooding and storms and can help in minimizing the loss of life and property. This main paper for the seminar proposes a [deep generative model to forecast precipitation from radar images](http://arxiv.org/abs/2104.00954). Ravuri et al. present a model that provides realistic and spatio-temporally consistent predictions over domains of up to 1536 km x 1280 km for lead times of 5 - 90 minutes.

The generative model has been shown to be skillful at probabilistic forecasting. It is evaluated qualitatively by human experts from the UK Met Office, and is found to be accurate and useful for actual operational application. We will also briefly cover existing approaches to precipitation nowcasting, following the review by [Prudden et al.](https://arxiv.org/abs/2005.04988).
<iframe width="560" height="315" src="https://www.youtube.com/embed/zLzGh8eIGfk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 28. "Learning to Precondition" 01.06.2021 

We will discuss the work of Ackmann et al. on using [machine learning to obtain fast preconditioners for (semi-)implicit numerical solvers](https://arxiv.org/abs/2010.02866), as used e.g. for the dynamical core of contemporary NWP systems. Solving systems of (linear) equations is a central task of such numerical solvers, and is typically tackled with iterative methods. To speed up convergence of these methods, [preconditioners](https://www.ecmwf.int/en/elibrary/12349-variational-methods-elliptic-problems-fluid-models) are used, and there is a sizeable literature on choosing efficient preconditioners for a given problem.

Ackmann et al. investigate the potential of learning data-driven preconditioners from numerical simulations. Their preconditioners are trained using the simple objective of predicting the state update between consecutive time points. They test their idea on the shallow water equations, and find that they can almost double the convergence speed of the linear solver using only linear models for the preconditioner.

<iframe width="560" height="315" src="https://www.youtube.com/embed/zSOvVOfohwk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 27. "Diving into Shallow Waters" 18.05.21

We will discuss Bihlo and Popovych’s work on [Physics-informed neural networks(PINNs) for the shallow-water equations](https://arxiv.org/abs/2104.00615) describing a hydrostatic fluid flow on the sphere. Their approach builds on the principles of Physics Informed Neural Networks and Fluid Mechanics as previously discussed in episodes 1 and 25.

The authors present an approach which involves training networks solely on the physical equations along with initial and boundary conditions but without any simulated data. These networks output  variables such as surface height and velocity as continuous functions of space and time.

The paper describes some interesting alterations to traditional PINNs such as non-dimensionalization of equations, splitting of the time domain, and projected gradients. These improved PINNs are then applied to various standard test cases to analyze performance on capturing phenomena such as advection, geostrophic flow, orographic flow and planetary waves. The results obtained from these tests present the ability of PINNs to capture physics-based constraints and allow for spatial continuity, implying the possibility of using them as a computationally cheaper alternative to traditional numerical weather prediction.


<iframe width="560" height="315" src="https://www.youtube.com/embed/877hwC7BShQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 26. "Learning the Rate of Change" 20.04.21

We will start by discussing the original paper introducing [Neural ODEs](https://arxiv.org/abs/1806.07366). The Neural ODE method builds on the similarity between Residual neural networks and Eulerian solvers for ODEs. This results in a model that is well-suited for taking on problems of forecasting, discontinuous data and speeding up solutions of differential equations--all of which are commonly encountered in Earth Science. We'll discuss the fundamentals of Neural ODEs and their various varieties, the structural differences from traditional ML, advantages and limitations over other ML methods and the scope of problems that can be solved using this method.

We will then discuss use cases of neural ODEs in the context of Earth Science. These include [turbulence forecasting](https://arxiv.org/abs/1911.05180), [hurricane nowcasting at irregular time steps](https://www.climatechange.ai/papers/iclr2020/21.html) and [crop classification under varying cloud cover](https://arxiv.org/abs/2012.02542), all of which highlight particular features of this method.

<iframe width="560" height="315" src="https://www.youtube.com/embed/EXIwS8fVCzA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe><br/>
<br/>


### 25. "Fluid Fluency" 06.04.21
We'll discuss [Learning Incompressible Fluid Dynamics from Scratch -- Towards Fast, Differentiable Fluid Models that Generalize](https://arxiv.org/abs/2006.08762).  

The Navier Stokes equations provide the foundation for much of fluid dynamics, and ultimately for models of the atmosphere and ocean. Wandel et al. describe a technique for solving the incompressible 2D NS equations using machine learning that combines important ideas from previous seminars and a number of remarkable new innovations. Like Physics Informed Neural Networks (PINNs, [ML Seminar 1](https://www.youtube.com/watch?v=p-B0_gk8Uj4)), this approach can be learned directly from the equations themselves, without requiring any numerical integrations as training data. 

Unlike PINNs, this new approach can also be applied to new initial conditions after training. We will discuss the mathematical tricks that went into its construction, consider its advantages and disadvantages, and review some of the spectacular fluid dynamics it can produce, including some challenging examples at high Reynolds numbers.

<iframe width="560" height="315" src="https://www.youtube.com/embed/IzJCeol-vSQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 24. "ML Jenga" 23.03.21

On Tuesday, March 23 at 3 PM (GMT+1), we will discuss the work of Franch et al. [Precipitation Nowcasting with Orographic Enhanced Stacked Generalization: Improving Deep Learning Predictions on Extreme Events](https://doi.org/10.3390/atmos11030267) and talk about their approach on creating an ensemble-based machine learning model for precipitation nowcasting with a focus on capturing extreme events.

Franch et al. use an ensemble of neural networks and stack them in a clever way, which is a common thing to do when applying machine learning models in practice, but it is rarely seen in research. We will cover why that is and what makes model stacking so useful. 

They also use a [newer version](https://arxiv.org/abs/1706.03458) of ConvLSTMs in an encoder-forecasting structure to do precipitation nowcasting. Because it has been nearly one year since we covered ConvLSTMs for precipitation forecasting in our seminar, we will give a little refresher on recurrent neural network architectures.

<iframe width="560" height="315" src="https://www.youtube.com/embed/RS_fkgiJV2A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 23. "Neural differential equations for Mixology" 09.03.21
On Tuesday, March 9 at 3 PM (GMT+1), we'll discuss "Capturing missing physics in climate model parameterizations using neural differential equations" [[paper]](https://arxiv.org/abs/2010.12559). 

This paper is about learning a convective adjustment parameterization within a simple ocean model [[website]](https://clima.github.io/OceananigansDocumentation/stable/gallery/).
Just like in our last seminar, the parameterization at hand is given by a differential equation, and the target of the ML model is its right-hand side. In this paper however, the authors make use of recent developments in the field of trainable differential equations [[paper]](https://arxiv.org/abs/2001.04385) to directly optimize over the solutions of the partial differential equation.

We will discuss the main paper and the underlying ML method "neural differential equations", and also have a quick look at the Oceananigans package used for the simulation.  
<iframe width="560" height="315" src="https://www.youtube.com/embed/yB_rl-6aUiU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 22. "Superdroplet Surprise" 23.02.21
On Tuesday, February 23 at 3 PM (GMT+1), we'll discuss "Potential and Limitations of Machine Learning for Modeling Warm-Rain Cloud Microphysical Processes."[paper](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2020MS002301) We're excited to announce that the first author, Axel Seifert from the German Weather Service (DWD), will be joining us!

This paper address the microphysical processes through which water droplets combine to form raindrops in clouds. While climate and weather models use simplified parametrizations such as bulk moment schemes to describe the complex evolution of the droplet size distribution over time, the computationally intensive superdroplet scheme[paper](https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/qj.441) can give a more precise and realistic answer. We will review the basics of these approaches before delving into the main paper.

This paper uses machine learning to train a fast surrogate for the superdroplet scheme. Surprisingly, while a neural network can learn a faithful bulk-moment representation of superdroplet physics, the simplified parameterization performs better at capturing the long term dynamics of the droplet size distribution. The reasons for this are explained by the paper, which reveals some counterintuitive and important insights that are bound to be highly relevant for the design of ML-based physical parametrizations in the future.
<iframe width="560" height="315" src="https://www.youtube.com/embed/rl4Wi-M6aNE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 21. "Lessons from History" 09.02.21
We discuss "Correcting weather and climate models by machine learning nudged historical simulations," Watt-Meyer et al., 2020. Geophysical Research Letters. [pdf](https://www.essoar.org/pdfjs/10.1002/essoar.10505959.1)

This paper addresses an important problem that has come up often in previous seminars, as well as in many internal discussions in our research group: how can we learn improved parameterizations and corrections for climate and weather model, without differentiating through the model's dynamics and physics? This is a very pressing issue in the near term as the gap between useful nondifferentiable models and differentiable toy models remains quite large.

This study offers a fresh and promising new approach. Instead of using expensive high-resolution simulations as training or imitating existing parameterizations with all their limitations, the authors propose learning additive corrections to the model so that it behaves more like an reanalysis dataset! We will discuss the specifics, advantages and limitations of this approach. The method uses random forests, which we covered previously in episode 19.

<iframe width="560" height="315" src="https://www.youtube.com/embed/KMNp2GN1ujY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 20. "Turning the Tide" 01.12.20
Zegou Zhang will present "Reconstruction of the Basin-Wide Sea Level Variability in the North Sea Using Coastal Data and Generative Adversarial Networks,"[pdf](https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/2020JC016402) recently published from the from the [Hydrodynamics and Data Assimilation](https://www.hereon.de/institutes/coastal_systems_analysis_modeling/hydrodynamics_data_assimilation/index.php.en) group at Hereon together with  Sebastian Grayek and Emil Stanev.

This paper uses adversarial networks to predict sea level across the North sea, and achieves excellent agreement with sophisticated operational forecasting systems by applying machine learning to only a small number of tidal gauge readings. It combines many important concepts we've seen in previous seminars, including forecasting, conditional GANs and U-nets. Unlike most of our previous papers, however, this work takes these concepts to the point of generating useful outputs for a real physical and geographic system.

Zegou will help us understand the data being used, the problem being solved, and how ML was applied. This presentation presents a great opportunity to ask questions to someone with hands on experience working with both oceanographic data and ML methods! 

<iframe width="560" height="315" src="https://www.youtube.com/embed/bT6xoOEIBlM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 19. "Durable Physics" 17.11.20
Shivani Sharma will present “Use of neural networks for stable, accurate and physically consistent parameterization of subgrid atmospheric processes with good performance at reduced precision,” Yuval et al., 2020.[pdf](https://arxiv.org/pdf/2010.09947.pdf)

As in Episode 10, this paper uses machine learning to replace physical parameterizations in an atmospheric model. However, the current paper is focused on a specific fundamental challenge: even when error appears low on training data with known inputs and outputs for the target parameterization, long-term simulations can “blow up” numerically, or exhibit unrealistic phenomena such as [grid scale storms](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018GL078510) or [double ITCZ](https://www.pnas.org/content/115/39/9684).

To overcome this “fragility” in the coupled simulations, the authors propose a “durable” approach incorporating physical constraints, prediction of fluxes instead of tendencies and careful selection of diagnostic variables. They demonstrate this strategy using both random forests (which we will briefly review) and neural networks. 
<iframe width="560" height="315" src="https://www.youtube.com/embed/9stE7uHyJuE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>


### 18. "Baking a Model from Scratch" 03.11.20
We discuss recent advances of using ML to learn dynamics from observational data.

In our last seminar, we already talked about transferring physical knowledge from a given dynamical model or parameterization to a ML model via training the latter on simulated data. An ambitious further step is to train an ML model directly on observational data, without the need of a physics-derived model of dynamics.

A big obstacle in this task is that observational data is usually noise-corrupted and incomplete. Our main paper for this week suggests to tackle this issue by combining ML with data assimilation. Using the Lorenz-96 model as a test-case, Brajard et al. [1] come up with an iterative method that uses an ensemble Kalman filter to provide better training data using a steadily improving neural network model of the system dynamics.

In a follow-up paper [2], which we will also briefly discuss, the authors explore a connection between their suggested method and Expectation-Maximization, a technique for optimizing statistical models in the presence of unobserved variables. This allows a Bayesian perspective on data-driven learning of dynamics.

Main paper:

[1] Brajard, J., Carassi, A., Bocquet, M., & Bertino, L. (2020). Combining data assimilation and machine learning to emulate a dynamical model from sparse and noisy observations: a case study with the Lorenz 96 model. [arXiv preprint arXiv:2001.01520](https://arxiv.org/abs/2001.01520).

Supporting paper:

[2] Bocquet, M., Brajard, J., Carrassi, A., & Bertino, L. (2020). Bayesian inference of chaotic dynamics by merging data assimilation, machine learning and expectation-maximization. Foundations of Data Science, 2(1), 55-80. [arXiv version](https://arxiv.org/abs/2001.06270)
<iframe width="560" height="315" src="https://www.youtube.com/embed/tgOwWMQHHc8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
<br/>
<br/>


### 17. "Radiation Computation" 20.10.20

The radiative transfer calculations in general circulation models often impose a computational challenge owing to the complexity of the current radiation models. This week, guest presenter Anikesh Pal (IIT Kanpur) will give an overview of these calculations, and describe his recent work at Oak Ridge National Laboratory on using neural networks to accelerate these computations.

In this study, deep neural networks (DNNs) were implemented in the Super‐Parameterized Energy Exascale Earth System Model (SP‐E3SM) to imitate the shortwave and longwave radiative transfer calculations. These DNNs were able to emulate the radiation parameters with an accuracy of 90–95% at a cost of 8–10 times cheaper than the original radiation parameterization. A comparison of time‐averaged radiative fluxes and the prognostic variables manifested qualitative and quantitative similarity between the DNN emulation and the original parameterization. It has also been found that the differences between the DNN emulation and the original parameterization are comparable to the internal variability of the original parameterization. Although the DNNs developed in this investigation emulate the radiation parameters for a specific set of initial conditions, the results justify the need of further research to generalize the use of DNNs for the emulations of full model radiation and other parameterization for seasonal predictions and climate simulations.

Main paper:

[1] Pal, Anikesh, Salil Mahajan, and Matthew R. Norman. "Using Deep Neural Networks as Cost‐Effective Surrogate Models for Super‐Parameterized E3SM Radiative Transfer." Geophysical Research Letters 46.11 (2019): 6069-6079.
[pdf](https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/2018GL081646)
<iframe width="560" height="315" src="https://www.youtube.com/embed/OjYhh68aXMg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### "Known Unknowns" 06.10.20
In our seminars so fo far we've considered many applications of supervised learning: given an input, our neural network is tasked with producing a correct output as demonstrated in a training set. However, as we have seen in some episdoes, in addition to predicting the correct output, neural networks can also quantify uncertainty, expressing how sure they are about their solution to the task at hand. Just like the accuracy of the network's predictions, we'd also like to quantify the accuracy of its uncertainty quantifications, asking in effect, "does the network know what it does and doesn't know?"

The [paper for this week](https://dl.acm.org/doi/pdf/10.5555/3305381.3305518) investigates this in the context of image classification (assigning the correct label from a finite list of categories to each image), and comes up with a surprising result. While neural networks have increased in overall classification accuracy over the past two decades, their uncertainty quantifications have actually gotten worse! In particular these networks have become overconfident. The paper investigates several changes in network architecture and training procedures that may play a role in this change, and proposes a simple and effective procedure for making them less overconfident without strongly affecting their accuracy.

[Main paper](https://dl.acm.org/doi/pdf/10.5555/3305381.3305518):
Guo, C., Pleiss, G., Sun, Y. & Weinberger, K. Q. On calibration of modern neural networks. in Proceedings of the 34th International Conference on Machine Learning - Volume 70 1321–1330 (JMLR.org, 2017).
<iframe width="560" height="315" src="https://www.youtube.com/embed/l2elXAnEKA4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### "Smooth Criminals" 15. 22.09.20
This week we discuss "Learning Temporal Coherence via Self-Supervision for GAN-based Video Generation" by Chu et al. 2020. [pdf](https://arxiv.org/pdf/1811.09393.pdf) [15]

They address the issue of GANs for video editing tasks usually would induce flickering or other artifacts. Thanks
to the spatio-temporal discriminator together with their “Ping-Pong loss” they outperform many previous approaches.

The results are presented on the tasks of unpaired video translation, as well as video super resolution. In our seminar
we will discuss how these techniques can be used in GANs for Earth-Science tasks.

[15] Chu, M., Xie, Y., Mayer, J., Leal-Taixé, L., & Thuerey, N. (2020). Learning temporal coherence via self-supervision for GAN-based video generation. ACM Transactions on Graphics (TOG), 39(4), 75-1.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PeP6wrTbWHo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 14. "When are we?" 08.09.20
We discuss "Viewing Forced Climate Patterns Through an AI Lens," Barnes et al. 2019 [pdf](https://agupubs.onlinelibrary.wiley.com/doi/pdf/10.1029/2019GL084944)

This paper takes up the task of finding features of meteorological fields (in this case temperature and precipitation) that be used to identify climate forcing (such as anthropogenic carbon emissions, or natural forcing due to volcanoes etc.).

The paper uses extremely small and simple feedforward neural networks, but with a clever trick -- it trains these networks to predict the year of a climate simulation with simulated anthropogenic forcing from the meteorological fields. Remarkably, when trained in the right way these same networks then perform well at identifying the year from these same fields in historical observational datasets! The simple neural networks are then analyzed to determine which features they have learned.
<iframe width="560" height="315" src="https://www.youtube.com/embed/xBV1MGu-JG0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 13. "Model Data for the Data Models" 25.08.20
We discuss "Purely data-driven medium-range weather forecasting achieves comparable skill to physical models at similar resolution," Rasp et al. 2020. This recent work builds machine learning tools for weather prediction to compete with physics based approaches. Stephan Rasp will return to the seminar to discuss his recent work on predicting temperature, geopotential and precipitation up to 5 days in the future, published just today on arXiv!

The [Weatherbench](https://arxiv.org/abs/2002.00469) benchmark for evaluating these techniques was proposed early this year, also by Rasp et al.
A key contributor to the performance increases in the current work was expanding the training available data beyond the weather that has actually occurred in the recorded past, by including other hypothetical situations realized through global climate modeling.

We discuss many conceptual and practical questions that arise when attempting to predict weather in this way, and consider what the future might hold for data-driven weather prediction.
<iframe width="560" height="315" src="https://www.youtube.com/embed/77aSvukSzL0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 12. "The Big Picture" 11.08.20
We discuss "Adversarial Super-resolution of Climatological Wind and Solar Data" [1], a recent study using Generative Adversarial Networks (GANs) with convolutional layers to increase the resolution of wind and irradiance fields output by climate models. This study uses high-resolution data to train a neural network to generate high-res from low-res data.

This week's topic is related to several previous themes: we covered GANs in episode 5 ("Real Fake Clouds"), and addressed a related problem of filling in missing data using convolutional networks in episode 8 ("Uncharted History").

We'll discuss the approach taken in this paper, describe the Machine Learning tool SRGAN which it uses [2], and debate the conceptual issues that arise when using ML to "invent" new pixel outputs for your model. We'll also mention how GAN-based superresolution can introduce bias into results [3], and what this could mean for climate and earth science applications.

Main paper:
[1] Stengel et al., “Adversarial super-resolution of climatological wind and solar data,” PNAS July, 2020. https://www.pnas.org/content/117/29/16805

Technical Background:
[2] Ledi et al., "Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network", arXiv 2016. https://arxiv.org/abs/1609.04802

Blog post on bias in GANs for SR:
[3] https://www.theverge.com/21298762/face-depixelizer-ai-machine-learning-tool-pulse-stylegan-obama-bias
<iframe width="560" height="315" src="https://www.youtube.com/embed/i4n28Xh_eQo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 11. "Teach Yourself Physics in 2 Million Easy Steps" 28.07.20
In this episode we discuss "Learning to Simulate Complex Physics with Graph Networks" [1], a recent study using deep learning to emulate physical dynamical systems.

We have already encountered several approaches to predicting physical systems in previous seminars (episodes 3, 4, 7 & 9). Typically, a machine learning model is trained on data generated with a numerical solver to predict a (partial) system state many time steps ahead, using the current (partial) system state as input. The network solves the task in a way that bears little, if any resemblance to the numerical solver used to generate its training data.

Here, the authors follow another approach [2], where the machine learning model is trained explicitly to reproduce or "emulate" the behavior of the numerical solver over individual numerical integration steps. We will discuss how learning to carry out single-time-step updates offers certain advantages over learning to predict the future directly from the present as the learning problem is very well posed conceptually and mathematically. However, a critical concern is whether the solutions of this 'learned simulation' stay realistic over many integration steps when using the emulator network instead of the numerical solver.

Another twist for the upcoming session will be that the dynamical systems studied are multi-body systems, i.e. they consist of a fixed number of discrete interacting objects. To learn state predictions on this kind of data, the authors designed their own Interaction Network [3], which is a subclass of so-called Graph Neural Networks. GNNs [4] have become a very active and vast topic of research over the past years that we can only briefly touch upon in our session.


Main paper:
[1] A. Sanchez-Gonzalez, J. Godwin, T. Pfaff, R. Ying, J. Leskovec, and P. W. Battaglia, “Learning to Simulate Complex Physics with Graph Networks,” arXiv:2002.09405 [physics, stat], Feb. 2020, Accessed: Jun. 27, 2020. http://arxiv.org/abs/2002.09405.

Additional Background:
[2] R. Grzeszczuk, D. Terzopoulos, and G. E. Hinton, “Fast Neural Network Emulation of Dynamical Systems for Computer Animation,” in Advances in Neural Information Processing Systems 11, M. J. Kearns, S. A. Solla, and D. A. Cohn, Eds. MIT Press, 1999, pp. 882–888. https://papers.nips.cc/paper/1562-fast-neural-network-emulation-of-dynamical-systems-for-computer-animation

[3] P. W. Battaglia, R. Pascanu, M. Lai, D. Rezende, and K. Kavukcuoglu, “Interaction Networks for Learning about Objects, Relations and Physics,” arXiv:1612.00222 [cs], Dec. 2016, Accessed: Jul. 16, 2020. [Online]. Available: http://arxiv.org/abs/1612.00222.

Further reading:
[4] J. Zhou et al., “Graph Neural Networks: A Review of Methods and Applications,” arXiv:1812.08434 [cs, stat], Jul. 2019, Accessed: Jul. 16, 2020. [Online]. Available: http://arxiv.org/abs/1812.08434.
<iframe width="560" height="315" src="https://www.youtube.com/embed/o7AwB-7TW-Y" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

### 10. "Try to look like a little black cloud" 14.07.20

In light of recent meteorological events in Hamburg, the next ML@HZG seminar will focus on clouds.

We will begin with a well-written 3-page review[1] that discusses how cloud resolving models (CRMs) can play an important role in our understanding of our climate and its potential changes in the future, but impose immense computational demands.

We'll then discuss how small-scale CRMs can be used as cloud parameterizations for large-scale climate models, focusing on the Superparameterized Community Atmosphere Model (SPCAM) [2]. This approach aims to capture the two-way interactions between cloud physics and coarser-scale meteorological variables without paying the cost of a huge CRM simulation, but instead embedding a small CRM into each grid cell. Further work[3] showed how the embedded CRMs can be simplified without compromising accuracy.

Finally, we'll discuss how machine learning can be used to imitate the effect of the miniature CRMs used in SPCAM, which in turn aims to imitate what a large-scale CRM might look like. Recent work[4] has shown the neural networks can be trained reproduce the feedback between coarse-scale climate model variables and each grid cell's CRM, with a considerable reduction of computational.

As we'll discuss, often the true test of these techniques is their ability to match observed phenomena in large, long simulations!

Postscript: as discussed in the seminar, it's not totally clear why the MJO moves east, but there are some interesting theories as to why[5] (thanks to Eduardo Zorita for the reference).

[1] T. Schneider et al., “Climate goals and computing the future of clouds,” Nature Clim Change, vol. 7, no. 1, pp. 3–5, Jan. 2017, doi: 10.1038/nclimate3190.

[2] M. Khairoutdinov, D. Randall, and C. DeMott, “Simulations of the Atmospheric General Circulation Using a Cloud-Resolving Model as a Superparameterization of Physical Processes,” J. Atmos. Sci., vol. 62, no. 7, pp. 2136–2154, Jul. 2005, doi: 10.1175/JAS3453.1.

[3] M. S. Pritchard, C. S. Bretherton, and C. A. DeMott, “Restricting 32–128 km horizontal scales hardly affects the MJO in the Superparameterized Community Atmosphere Model v.3.0 but the number of cloud-resolving grid columns constrains vertical mixing,” Journal of Advances in Modeling Earth Systems, vol. 6, no. 3, pp. 723–739, 2014, doi: 10.1002/2014MS000340.

[4] S. Rasp, M. S. Pritchard, and P. Gentine, “Deep learning to represent subgrid processes in climate models,” PNAS, vol. 115, no. 39, pp. 9684–9689, Sep. 2018, doi: 10.1073/pnas.1810286115.

[5] B. Wang, F. Liu, and G. Chen, “A trio-interaction theory for Madden–Julian oscillation,” Geosci. Lett., vol. 3, no. 1, p. 34, Dec. 2016, doi: 10.1186/s40562-016-0066-z.
<iframe width="560" height="315" src="https://www.youtube.com/embed/XyPLZbQ3Fps" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>
<br/>

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
