---
permalink: /
title: "About me"
excerpt: "Learn about DGK"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a student at [Albert Einstein College of Medicine](https://einsteinmed.edu/) (expected MD 2024) and a recent graduate of the [Certificate in Premedical Sciences](https://gs.columbia.edu/content/postbac-premed-program) program of Columbia University. I am interested in the application of mathematics and technology to medicine and am a current research assistant in the [Crary Lab](http://www.crarylab.org/home.html) at Mount Sinai studying applications of machine learning in neuropathology. I have previous research experience in Combinatorics and Astrophysics. I worked as a software engineer in scalable data infrastructure at a native advertising start up called [Triplelift](https://triplelift.com/). I also write poetry, music, and short stories. 

## Bragging Rights: 
* [Submitted a Correction to AMBOSS](/files/AmbossProof.png)
* Made this website and my [wedding website](https://danielkirsten.com)
* I own my very own [canoe](/files/canoeproof.jpg) 
* I love my [pets](/files/birthdaydogandcat.jpg) and [travel](/files/lilycold.jpg) with them 

## Einstein Ad Libitum: 
* [Website](https://www.einsteinmed.edu/students/clubs/ad-libitum/default.aspx?id=15486) 
* [Vol 19 Spring 21 (Two Poems)](https://www.einsteinmed.edu/docs/Students/Clubs/Ad-libitum/ad-libitum-2021.pdf) 

## Coursework Projects: 

<details open> 
<summary>Computational Neuroscience 2018</summary>

In one of my favorite classes we were asked as a final project to create a neural encoder utilizing a spectrotemporal filter and array of <a href="https://mathematical-neuroscience.springeropen.com/articles/10.1186/2190-8567-1-7">Noisy Leaky IAF</a> "trigger and fire" neurons. The leaky IAF is an encoder of a signal into a train of spikes that is meant to approximate the traditional Hodgkin and Huxley neuron quite well by preserving the nonlinear nature of the Hodgkin and Huxley neuron without the sacrifice of needless computation time. In this way neurons translate amplitude signals into a frequency based sampling space. 

<p align="center">
  <img src="/images/CircuitEncoder.png">
</p> 

Above is a schema of the proposed project. A signal is passed in the two dimensional space of frequency and time into the spectrotemporal filter. The resulting signal is added to a bias and fed through the leaky IAF. The claim is that using the right analysis (handwaving aside) we can mathematically recompute the filter from the spike train. This same method of inquiry could in theory be applied to real neurons in order to determine the filtering occurring at the axon hillock. 

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

Once we have the spike times, we are able to recover an approximation of the spectrotemporal filter. Some discrepancies exist where the filter value changes suddenly (i.e. where it approaches its minimum of -10). This is because in the filter is effectively zeroes and its bandwidth is effectively infinite. This method is limited computationally wherever the bandwidth is sufficiently high, however the approximation of the filter is still quite good. This approach can be used to describe neurological phenotypes in various disease states <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2474630/">(as is the case here)</a>. 
</details> 
<details open> 
<summary>Advanced Physics Lab 2013</summary> 

In one of my favorite experiments way back in college we were tasked with building a <a href="https://en.wikipedia.org/wiki/PID_controller#:~:text=A%20proportional%E2%80%93integral%E2%80%93derivative%20controller,continuously%20calculates%20an%20error%20value">PID controller</a>. The idea behind the PID controller is that you have a real value you want your program to accomplish but you only have access to some kind of power which moves you in the direction of that real world value. In the real world things like momentum, resistance, and error complicate problems and simply setting your power proportional to the difference between your desired real world value and the current one doesn't work optimally. Take for instance an air conditioning unit. The AC unit only knows different power settings, what the current temperature is, and what the desired temperature is. If it rapidly cools down a room to a desired temperature it may overshoot. The process of optimally approaching a given value is far more important when applied to autopilot systems or robots used in surgery. 

<p align="center">
  <img src="/images/PIDDiagram.png">
</p>

In a PID controller the difference between your desired value and your current value is referred to as the error (this can be confusing because there is probably error between your current value and your measured current value). We set our power proportionally to the error, the integral of the error over time, and the derivative of the error over time (all approximated numerically). 

<p align="center">
  <img src="/images/PIDControllerFunction.png">
</p>

This gives us an equation with a bunch of mysterious constants. The job of optimally determining the best values has been done for us by <a href="https://en.wikipedia.org/wiki/Ziegler%E2%80%93Nichols_method">Ziegler and Nichols</a>. We must simply find the value for which the proportional portion of our PID creates a simple wave. This can be done by fine tuning and inspection, or robustly it can be done by taking the fast Fourier transform of the data and finding the frequency with the highest peak. 

<p align="center">
  <img src="/images/PIDSetup.jpg">
</p>

The experiment was conducted and programmed in labVIEW where a given temperature was set for a <a href="https://en.wikipedia.org/wiki/Thermoelectric_generator">thermoelectric generator</a>. 

<p align="center">
  <img src="/images/FinalPID.jpg">
</p>

In the above there is a tight approximation of 35 degrees Celsius by the PID controller (top right). The fast Fourier transform is also displayed showing a peak of about 3.2 Hz (bottom left). This enabled us to optimally set the coefficients (right side) and build a very reactive PID controller. 
</details> 

## MOTIVATE Lab: 
* [About Me](https://med.nyu.edu/jaylab/team-alumni) 
