---
permalink: /
title: "About me"
excerpt: "Learn about DGK"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a student at [Albert Einstein College of Medicine](https://einsteinmed.edu/) (expected MD 2024) and a recent graduate of the [Certificate in Premedical Sciences](https://gs.columbia.edu/content/postbac-premed-program) program of Columbia University. I am interested in the application of mathematics and technology to medicine and am a current research assisstant in the [Crary Lab](http://www.crarylab.org/home.html) at Mount Sinai studying applications of machine learning in neuropathology. I have previous research experience in Combinatorics and Astrophysics. I worked as a software engineer in scalable data infrastructure at a native advertising start up called [Triplelift](https://triplelift.com/). I also write poetry, music, and short stories. 

## Online CVs 
* [Google Scholar](https://scholar.google.com/citations?user=A_xgHTAAAAAJ&hl=en&oi=ao)
* [LinkedIn](https://www.linkedin.com/in/daniel-koenigsberg) 
* [AngelList](https://angel.co/daniel-koenigsberg) 

## Einstein Ad Libitum: 
* [Website](https://www.einsteinmed.edu/students/clubs/ad-libitum/default.aspx?id=15486) 
* [Vol 19 Spring 21 (Two Poems)](https://www.einsteinmed.edu/docs/Students/Clubs/Ad-libitum/ad-libitum-2021.pdf) 

## MOTIVATE Lab: 
* [About Me](https://med.nyu.edu/jaylab/team-alumni) 

## Bragging Rights: 
* [Submitted a Correction to AMBOSS](/files/AmbossProof.png)

## Coursework Projects: 

### Computational Neuroscience 

In one of my favorite classes we were asked as a final project to create a neural encoder utilizing a spectrotemporal filter and array of Leaky IAF "trigger and fire" neurons. 

<p align="center">
  <img src="/images/tem-iaf-rt.png">
</p>

The leaky IAF is an encoder of a signal into a trian of spikes that is meant to approximate the tradiational Hodgkin and Huxley neuron quite well, by preserving the nonlinear nature of the Hodgkin and Huxley neuron without the sacrifice of needless computation time. In this way neurons translate amplitude signals into a frequency based sampling space. 

<p align="center">
  <img src="/images/CircuitEncoder.png">
</p> 

Above is a schema of the proposed project. A signal is passed in the two dimensional space of frequency and time into the spectrotemporal filter. The resulting signal is added to a bias and fed through the leaky IAF. The claim is that using the right analysis (handwaving aside) we can mathematically recompute the filter from the spike train. This same method of inquiry could in theory be applied to real neurons in order to determine the filtering occuring at the axon hillock. 

<p align="center">
  <img src="/images/STRF%20Initial%20Filter.png">
</p>

Above is a diagram of the initial spectrotemporal filter. Different two dimensional and three dimensional views are provided. 

<p align="center">
  <img src="/images/LeakyIAFEncoding.png">
</p>

Above is the resulting spike train of passing the signal (on top) through the circuit and adding noise proportional to the firing threshold. 

<p align="center">
  <img src="/images/RecoveredFilter.png">
</p>

Once we have the spike times we are able to recover an approximation of the spectrotemporal filter. Some discrepancies exist where the filter value was zeroed. This is because in the filter the bandwidth is effectively infinite. The method is limited computationally whereever the bandwidth is too high, however the approximation of the filter is still quite good. 
