---
layout: single
title:  "Research Theme: Modeling the gravitational-wave memory signal"
date:   2026-09-07
categories: papers
---

This post describes two papers on constructing gravitational waveform models for the gravitational-wave memory effect. 

## Papers Highlighted ##

* A. Elhashash and **D. A. Nichols**.
"Waveform models for the gravitational-wave memory effect: III. Phenomenological frequency-domain model for nonspinning binaries."
[arXiv:2609.04340](https://doi.org/10.48550/arXiv.2609.04340).

* A. Elhashash and **D. A. Nichols**.
"Waveform models for the gravitational-wave memory effect: II. Time-domain and frequency-domain models for nonspinning binaries."
[Phys. Rev. D 112, 064014 (2025)](https://doi.org/10.1103/wzqk-62wc).
[arXiv:2504.18635](https://doi.org/10.48550/arXiv.2504.18635).

* A. Elhashash and **D. A. Nichols**.
"Waveform models for the gravitational-wave memory effect: Extreme mass-ratio limit and final memory offset."
[Phys. Rev. D 111, 044052 (2025)](https://doi.org/10.1103/PhysRevD.111.044052).
[arXiv:2407.19017](https://doi.org/10.48550/arXiv.2407.19017).

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

The most recent pre-print (the third paper in the series) took a different approach than the time-domain model in the second paper.
Whereas the time-domain model in the second paper used analytical calculations of the inspiral and ringdown memory signals with a phenomenological expression for the times between the late inspiral and the start of the ringdown, in this most recent paper, we instead used smooth frequency-domain functions that matched the qualitative properties of the memory signal in frequency space (namely, it goes as one over frequency at low frequencies and decays exponentially with frequency for frequencies larger than the inverse of the typical time scale over which the memory signal accumulates).
One advantage of this more phenomenological approach was that the frequency-domain signal could be represented in simpler analytical functions than the special functions used to represent the analytical Fourier transform of the time-domain model from the second paper.
This allowed the model to be computed more efficiently than the previous time-domain model.
A second advantage, is that the inverse Fourier transform of the frequency-domain model is a smooth function in the time domain.
The time-domain model of the second paper, however, had only a finite degree of differentiability at the two points where the inspiral and ringdown models matched to the intermediate section of the time-domain model.
This finite degree of differentiability also introduced high-frequency artifacts into the frequency-domain representation of the time-domain model of the second paper, which limited this model's accuracy.
