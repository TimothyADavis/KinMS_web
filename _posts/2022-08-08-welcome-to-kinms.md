---
layout: post
title: "What is KinMS?"
author: "Tim Davis"
categories: documentation
tags: [documentation,sample]
image: KinMS_fade_gal.png
permalink: '/welcome-to-kinms'
---


The KinMS set of packages can be used to forward model 3D datacubes from interferometers and/or Integral Field Units (IFUs); or, with some postprocessing, 1D/2D data products and long-slit spectra. 

KinMS standards for "KINematic Molecular Simulation", as modelling the kinematics of molecular gas data was the original usecase (e.g. investigating the kinematics of gas in early-type galaxies, [Davis et al., 2013a](https://academic.oup.com/mnras/article/429/1/534/1022845); and determining supermassive black-hole masses from interferometric observations, [Davis et al., 2013b](https://ui.adsabs.harvard.edu/abs/2013Natur.494..328D/abstract)), but KinMS is useful for a wide variety of use cases beyond this. Some examples from the [40+ peer reviewed papers that use KinMS](https://ui.adsabs.harvard.edu/search/filter_property_fq_property=AND&filter_property_fq_property=property%3A%22refereed%22&fq=%7B!type%3Daqp%20v%3D%24fq_property%7D&fq_property=(property%3A%22refereed%22)&q=%20full%3A%22KinMS%22&sort=date%20desc%2C%20bibcode%20desc&p_=0) include:

* Creating mock datacubes from hydrodynamic simulations: [Davis et al. 2019](https://ui.adsabs.harvard.edu/abs/2019MNRAS.484.2447D/abstract)
* Modelling optical ionised-gas line profiles from MaNGA IFU/long-slit spectra in Red Geysers: [Roy et al. 21](https://ui.adsabs.harvard.edu/abs/2021ApJ...913...33R/abstract)
* Modelling the kinematics of edge on disc galaxies to search for non-circular motions: [Hogarth et al. 2022](https://arxiv.org/abs/2204.02925)

<font size=1>(If you have used KinMS for something particularly outside of the ordinary let me know- I'd be delighted to feature you here!)</font>

### Why choose KinMS?

Various kinematic modelling packages are available, and widely used in the astronomical community. For instance [TiRiFiC](https://gigjozsa.github.io/tirific/), [3D-Barolo](https://editeodoro.github.io/Bbarolo/) and [GalPaK3D](http://galpak3d.univ-lyon1.fr/). Each has its own strengths and weaknesses, and may be better/worse for your specific problem. Here I outline some of the advantages of KinMS, so you can determine if it is the package for you:

* <b><u>KinMS allows you to go beyond tilted rings.</u></b> It can be used as a classic tilted ring fitting code (but if that is your main use case and you don't need any of KinMS's extra functionality I recommend either TiRiFiC or 3D-Barolo), but shines when used to fit physically motivated functional forms for e.g. rotation curves and/or gas surface brightness profiles. For instance, it includes models for various potentials, allowing kinematic disc-bulge decompositions, the inclusion of compact objects, using [MGE decompositions](https://www-astro.physics.ox.ac.uk/~cappellari/software/#mge) of stellar light, etc.
* <b><u>KinMS is flexible.</u></b> It can be used to fit non-axisymmetric structures such as spirals, bars and merging galaxies via its `inClouds` mechanism, and allows the user significant freedom in the types of circular/non-circular motions modelled. 
* <b><u>KinMS is Bayesian.</u></b> By default the `KinMS_fitter` routines use a Markov Chain Monte Carlo (MCMC) approach, allowing the user to set arbitrary priors, explore degeneracies and obtain full ND posterior probability distribution functions. 
* <b><u>KinMS is implemented in pure python.</u></b> This makes it simple to understand and use (to e.g. build a pipeline for fitting many objects), easy to modify for your needs (e.g. if you need to move beyond simple disc fitting), and effortless to install across different environments.  

If some or all of this sounds good, then go to the [Installation & Tutorial]({{ site.github.url }}{% post_url 2022-08-07-getting-started_wkinms %}). If you are still unsure then feel free to [contact me]({{ site.github.url }}/about). 