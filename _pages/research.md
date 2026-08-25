---
title: "Research"
permalink: /research/
---

My PhD research focuses on high-accuracy numerical methods for black hole perturbation theory, with applications to gravitational wave physics, extreme mass ratio inspirals (EMRIs), and horizon-scale phenomena in extremal black holes.

## Research Highlights

### 1. Discontinuous Galerkin methods for singular-source Teukolsky evolutions

![DG Teukolsky waveform convergence summary](/images/research/teukolsky-dg-waveform.png)
*Figure: Schematic convergence behavior for waveform extraction in singular-source Teukolsky evolutions.*

EMRIs are key targets for **[LISA](https://www.lisamission.org/)** and require accurate time-domain solutions of the **[Teukolsky equation](https://ui.adsabs.harvard.edu/abs/1973ApJ...185..635T/abstract)**. I develop **[discontinuous Galerkin (DG)](https://link.springer.com/book/10.1007/978-0-387-72067-8)** methods that directly handle distributional particle sources, avoiding narrow-Gaussian regularization errors and improving convergence near the source.

**Related links:** [Paper](/publication/paper-1)

### 2. Radiation outer boundary conditions for long-time stable simulations

![ROBC stability and reflection suppression schematic](/images/research/bp-robc-stability.png)
*Figure: Schematic comparison showing reduced boundary reflections and stable long-time decay with ROBC kernels.*

Long-duration simulations on finite domains are often contaminated by spurious reflections and late-time artifacts under standard outgoing boundary conditions. I investigate exact radiation boundary kernels and hyperboloidal-inspired strategies for the Bardeen–Press equation to enable stable long-time evolution and accurate asymptotic waveform recovery.

**Related links:** [Paper](/publication/paper-3) · [ICERM poster](/images/ICERM_SciML_inGWs_Poster.pdf)

### 3. Horizon hair as a potential observable of extremal black holes

![Extremal horizon hair signal imprint schematic](/images/research/extremal-hair-signal.png)
*Figure: Schematic late-time signal behavior highlighting conserved-hair imprints in near-horizon dynamics.*

While classical no-hair results characterize stationary black holes by mass, spin, and charge, extremal Kerr geometries exhibit conserved horizon quantities for specific perturbations. I study how these scalar/gravitational hair signatures can propagate into measurable waveform features and distinguish extremal from sub-extremal systems.

**Related links:** [Paper](/publication/paper-2) · [Talk slides](https://drive.google.com/file/d/1_HpPvOZMyCARq1e6Az1E-CN33IHNGBKC/view?usp=sharing)

---
*Last updated: August 2026*

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


**Content on this page will change with increasing clarity and conciseness**




 -->