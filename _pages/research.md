---
title: "Research"
permalink: /research/
---

# Research

My PhD research focuses on developing high-accuracy numerical methods for black hole perturbation theory, with applications to gravitational wave physics, extreme mass ratio inspirals (EMRIs), and the structure of black hole horizons.

### 1. Discontinuous Galerkin Methods for the Teukolsky Equation with Singular Sources on Generic Orbits

Extreme mass ratio inspirals (EMRIs) — systems involving a stellar-mass compact object orbiting and plunging into a supermassive black hole — are prime targets for the **Laser Interferometer Space Antenna (LISA)**. These systems are accurately described within black hole perturbation theory, where the gravitational radiation is governed by the **Teukolsky equation**.

The source term in the Teukolsky equation for a point particle includes derivatives of the Dirac delta function, traditionally approximated by a narrow Gaussian. This approximation introduces systematic errors and limits convergence, especially for realistic (eccentric or generic) orbits.

I am developing a **discontinuous Galerkin (DG)** finite element method that directly incorporates the distributional singular source without regularization. This approach achieves **spectral accuracy** even near the singularity, enabling exponentially convergent waveforms and self-force calculations for progressively more realistic EMRI orbits.

### 2. Exact Outer Boundary Conditions for the Bardeen–Press Equation

The **Bardeen–Press equation** is the spin-0 (scalar) counterpart of the Teukolsky equation on Schwarzschild spacetime, describing gravitational perturbations around non-rotating black holes.

Long-time numerical evolutions of wave equations on unbounded domains suffer from spurious reflections and late-time instabilities when using standard Sommerfeld (outgoing) boundary conditions.

I am investigating advanced non-reflecting boundary techniques, including **hyperboloidal compactification** (inspired by methods related to perfectly matched layers / Berenger-type absorbers) and boundary integral kernels. These approaches map null infinity to a finite coordinate location, eliminating artificial boundaries and ensuring long-term stability and accurate extraction of gravitational waveforms at future null infinity.

### 3. Observational Signatures of Gravitational Hair in Extremal Kerr Black Holes

The **no-hair theorem** asserts that stationary black holes in general relativity are fully characterized by their mass, spin, and charge — with no additional independent parameters (“hair”).

However, for scalar fields (and potentially gravitational perturbations) in extremal Kerr spacetimes (maximally spinning, a = M), certain quantities on the event horizon fail to decay at late times and remain conserved. These conserved charges can distinguish extremal from sub-extremal black holes, potentially violating the classical no-hair picture in the extremal limit.

I am exploring the nature of this **horizon hair** (both scalar and gravitational), its conservation properties, and possible observational imprints in gravitational wave signals — especially whether such features could leave detectable signatures in waveforms from near-extremal systems.

<!-- 
# 1. Solving the Teukolsky equation with singular source terms for generic orbits

* Laser Interferometer Space Antenna will detect gravitational waves from Extreme Mass Ratio Inspirals. These systems are described by black hole perturbation theory due to the disparate sizes of the two bodies. The dynamics of these waves is governed by the Teukolsky equation. 

* Teukolsky equation has to be solved with source terms with derivatives of the Dirac delta function which is traditionally modelled as a narrow Gaussian. This delta function models a particle in a particular kind of orbit such as circular, eccentric, generic.

* I use discontinuous Galerkin methods to incorporate this singular 
source term and get spectral accuracy in the numerical solution. Aim is to do this for progressively realistic EMRI orbits.


# 2. Exact outer boundary conditions for the Bardeen-Press equation

* The Bardeen-Press equation is spin 0 or Schwarzschild version of the Teukolsky equation. It describes gravitational perturbations in the spacetime of Schwarzschild black holes, while the Teukolsky equation describes perturbations of Kerr black holes.

* Long simulations of these equations require accurate non-reflecting outer boundary condtions since using Sommerfeld BCs suffer from instabilities at late times.

* I am exploring different techniques such as hyperboloidal compactification (based on the perfectly matched layers technique by Berenger) and boundary kernels to get rid of spurious reflections and
long time stability.


# 3. Observational implications for Gravitational hair from extremal Kerr black holes 

* The no-hair theorem in general relativity states that a black hole is fully characterized by three parameters namely the mass, spin and charge. In that sense there are no other(independent) quantities that can distinguish between two black holes.

* For a scalar field in a BH spacetime, there are quantities on the event horizon that fail to decay at late times i.e. they are conserved
on the horizon. 

* These conserved charges have the ability to distinguish extremal (i.e. maximally spinning where a=M) from sub-extremal black holes (where a<M). Here a is the spin of the black hole and M its mass. 


**Content on this page will change with increasing clarity and conciseness** -->