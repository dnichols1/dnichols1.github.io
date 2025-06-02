---
layout: single
title:  "Research Theme: Modeling the gravitational-wave memory signal"
date:   2025-04-25
categories: papers
---

This post describes two papers on constructing gravitational waveform models for the gravitational-wave memory effect. 

## Papers Highlighted ##

* A. Elhashash and **D. A. Nichols**.
"Waveform models for the gravitational-wave memory effect: II. Time-domain and frequency-domain models for nonspinning binaries," (2025).
[arXiv:2504.18635](https://arxiv.org/abs/2504.18635).

* A. Elhashash and **D. A. Nichols**.
"Waveform models for the gravitational-wave memory effect: Extreme mass-ratio limit and final memory offset."
[Phys. Rev. D 111, 044052 (2025)](https://doi.org/10.1103/PhysRevD.111.044052).
[arXiv:2407.19017](https://arxiv.org/abs/2407.19017).

## Summary of the Papers ##

![](/images/memoryEMRI.png){: .align-left}
As discussed in other posts on this webpage, the gravitational-wave memory effect is a prediction of general relativity that is closely connected to the symmetries and conservation laws of asymptotically flat spacetimes.
Its most prominent feature is a lasting offset in the gravitational-wave strain that persists after a burst of waves passes by a detector.
Pulsar timing arrays, for example, perform searches for bursts of gravitational waves with memory by looking for the effect of this offset on the arrival times of radio pulses from pulsars.

For interferometers, such as LIGO and Virgo, the lasting offset itself is challenging to measure, because of they are limited in the lowest frequency of gravitational waves that they can confidently detect.
However, there is a well-defined time-dependent portion of the gravitational-wave signal that produces the lasting offset, which the LIGO and Virgo detectors likely will be able to measure (in a statistical sense, across the entire population of black-hole mergers that the detectors measure).
The algorithms that search for the memory effect evaluate the waveform a very large number of times, so it is advantageous to have a model of the time-domain signal that can be evaluated more quickly.
In addition, these analyses are performed in the frequency domain, so it can also be helpful to have a frequency-domain model, so as to avoid performing the fast Fourier transform and the associated signal processing of the time-domain memory signal that is required to avoid certain data artifacts.

In the first of the two papers, we computed the memory offset for non-spinning binary black holes.
We performed a new calculation of the time-domain memory signal for extreme mass-ratio inspirals, using a high post-Newtonian-order approximation, which we incorporated into our memory offset model.
The second of the two papers used the offset model, combined with post-Newtonian and black-hole-perturbation theories, to compute an analytical waveform model for the time-domain memory signal.
This time-domain model also had an analytical Fourier transform, which gave us a frequency-domain model for non-spinning binary black holes.
The models were calibrated up to a mass ratio of eight.
