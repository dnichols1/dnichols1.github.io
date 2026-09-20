---
layout: single
title:  "Research Theme: Hybrid Post-Newtonian and Black-Hole Perturbation Model"
date:   2026-05-26
categories: papers
---

This post is a summary of two papers I wrote with Yanbei Chen during my Ph.D. about a semi-analytical model for explaining the properties of the gravitational waveforms from binary-black-hole mergers. Recently, Nur Rifat, Kent Yagi, and I wrote a third paper that modified this model to allow for more accurate waveform modeling.

## Papers Highlighted

* N. E. M. Rifat, **D. A. Nichols** and K. Yagi.
"Hybrid model for inspiral-merger-ringdown gravitational waveforms from comparable-mass, nonspinning binary black holes."
[Phys. Rev. D 113, 104051 (2026)](https://doi.org/10.1103/2b54-gscd)
[arXiv:2511.09646](https://doi.org/10.48550/arXiv.2511.09646)

* **D. A. Nichols** and Y. Chen. 
"Hybrid method for understanding black-hole mergers: Inspiralling case." 
[Phys. Rev. D 85, 044035 (2012)](http://dx.doi.org/10.1103/PhysRevD.85.044035),
[arXiv:1109.0081](https://doi.org/10.48550/arXiv.1109.0081).

* **D. A. Nichols** and Y. Chen. 
"Hybrid method for understanding black-hole mergers: Head-on case." 
[Phys. Rev. D 82, 104020 (2010)](http://dx.doi.org/10.1103/PhysRevD.82.104020),
[arXiv:1007.2024](https://doi.org/10.48550/arXiv.1007.2024).

## Summary of the Papers

![](/images/hybridUV.png){: .align-left}
While it is now feasible to compute the merger of black holes with large-scale simulations, it is still helpful to use analytical methods to develop faster ways of calculating gravitational waveforms and to provide intuitive understanding of these processes. 
We put forward a method of combining two analytical approximation schemes—Post-Newtonian (PN) and black-hole-perturbation (BHP) theories—to make approximate gravitational waveforms and to clarify the structure of a black-hole-binary merger.
The central idea of the method is to use both PN and BHP theories simultaneously at a given time, but to restrict their use to spatial regions where either they are good approximations or their errors will not effect important observables like the gravitational waveform.
Typically, PN and BHP theories are applied to the entire spatial region of distinct times in the evolution of a binary.

Applying both PN and BHP theory at once requires there be a region where one can match the two theories. 
We found empirically that we can match the theories at the locations of the PN theory's point particles. 
We then let the matching region evolve by requiring that the point particles follow a combination of geodesic motion in the final black-hole's background and dissipative motion from a radiation-reaction force (which was calculated self-consistently from the emitted gravitational waves). 
This new set of evolution equations simultaneously computes the matching region and the gravitational waves outside of it. 
The waveform that they produce is not calibrated to numerical simulations, but still captures the qualitative behavior of the waveforms for both head-on and quasi-circular binaries.
The method was also useful for exploring how black holes get large recoil velocities when they have spin vectors that are anti-aligned in the orbital plane.

Because the agreement between the hybrid method and numerical relativity results was not precise, Nur Rifat, Kent Yagi, and I recently investigated what changes to the method are needed to make it better agree with numerical relativity results.
We found that the method could be adapted to match more precisely if the following three changes were made.
First, we needed to use the effective-one-body method to describe the motion of the point particles to obtain better agreement in the gravitational-wave phase during the inspiral.
Second, the value of the boundary data at the matching region needed to be modified with two parameters, so as to make the amplitude during the inspiral and merger more closely match the waveforms from numerical-relativity simulations.
Third, the effective potential in the BHP spacetime needed to be altered, so that they were in better correspondence with the dominant ringdown frequency and damping time of the least-damped quasi-normal mode of the remnant black hole.
With these three modifications, the hybrid method could be calibrated to agree with numerical relativity results for non-spinning binaries with mass ratios between one and eight.
