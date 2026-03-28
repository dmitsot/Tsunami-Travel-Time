# Tsunami Travel Time

This Jupyter notebook provides a practical framework for computing tsunami travel-time isolines and estimating the arrival time of a tsunami at a given location. By using the capabilities of the scikit-fmm module, it efficiently solves the underlying eikonal equation that estimates wavefront propagation. This implementation is based on the fast marching method proposed by James Sethian for solving boundary value problems of the Eikonal equation. (For more information see "J.A. Sethian. A Fast Marching Level Set Method for Monotonically Advancing Fronts, Proc. Natl. Acad. Sci., 93, 4, pp.1591--1595, 1996").

The arrival time or travel time is the time taken for the leading edge (or wavefront) of the tsunami to travel from the origin, such as an undersea earthquake, to a given point of interest. This is what the notebook computes when solving the underlying propagation problem.

It is important to distinguish this from other possible interpretations:

- It does not necessarily correspond to the time of the largest wave or peak amplitude.
- It represents the earliest detectable signal, which is often the most relevant quantity for early warning systems.
- In mathematical terms, it is the travel time obtained from the solution of the eikonal equation, assuming wave speed depends on local water depth.

The notebook is designed to be both accessible and flexible: users can input location data and source parameters, visualize the resulting travel-time contours, and extract quantitative arrival-time estimates for points of interest within minutes. As such, it serves not only as a computational tool but also as a means to explore how seabed topography influences tsunami propagation across ocean basins.

Disclaimer. This code is not intended to predict or forecast tsunami events. The computed results are approximate and rely on simplifying assumptions, such as idealized wave propagation and the quality of the input data. Consequently, the estimated arrival times should be interpreted as indicative rather than definitive, and they should be used with caution.

![tsunami_travel_time_simple](https://github.com/user-attachments/assets/882aef26-47c7-4d34-8f95-5de1723beb57)

![tsunami_travel_time](https://github.com/user-attachments/assets/b42a48ea-d207-49c8-b244-2d092ec86fad)

