---
title: "Radiation Outer Boundary Conditions for the Teukolsky equation"
collection: talks
type: "Contributed Talk"
permalink: /talks/2026-03-18-talk-ROBC-aps
venue: "APS Global Physics Summit 2026"
date: 2026-03-18
location: "Denver, Colorado"
---

This talk presents my recent work on radiation outer boundary conditions for the Bardeen-Press equation. This technique helps us to solve the BP equation in the time domain but with a much smaller computational domain. This helps in producing high resolution simulations efficiently, since we can have $\Delta x$ and $\Delta t$ small. Without this technique, a smaller computational domain would lead to spurious reflections from the outer boundary, which can contaminate the true physical solution.

Using the technique of teleportation, we can extract the solution at a finite radius and then teleport it to infinity, which is the physical location where we want to measure the gravitational wave signal. This allows us to obtain accurate waveforms without having to simulate the entire spacetime out to infinity.