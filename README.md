# Tsunami Travel Time

This Jupyter notebook provides a practical framework for computing tsunami travel-time isolines and estimating the arrival time of a tsunami at a given location. By leveraging the capabilities of the scikit-fmm module, it efficiently solves the underlying eikonal equation that governs wavefront propagation.

The arrival time or travel time is the time taken for the leading edge (or wavefront) of the tsunami to travel from the origin—such as an undersea earthquake—to a given point of interest. This is what the notebook computes when solving the underlying propagation problem.

It is important to distinguish this from other possible interpretations:

- It does not necessarily correspond to the time of the largest wave or peak amplitude.
- It represents the earliest detectable signal, which is often the most relevant quantity for early warning systems.
- In mathematical terms, it is the travel time obtained from the solution of the eikonal equation, assuming wave speed depends on local water depth.

The notebook is designed to be both accessible and flexible: users can input location data and source parameters, visualize the resulting travel-time contours, and extract quantitative arrival-time estimates for points of interest in minutes. As such, it serves not only as a computational tool but also as a means to explore how seabed topography influences tsunami propagation across ocean basins.

Disclaimer. This code is not intended to predict or forecast tsunami events. The computed results are approximate and rely on simplifying assumptions, such as idealized wave propagation and the quality of the input data. Consequently, the estimated arrival times should be interpreted as indicative rather than definitive, and they should be used with caution.

<img width="1360" height="1035" alt="tsunami_travel_time_simple" src="https://github.com/user-attachments/assets/6a6e4205-d76a-429b-8048-bcac4235be7d" />
<img width="1693" height="1180" alt="tsunami_travel_time" src="https://github.com/user-attachments/assets/1c632a1b-e53e-4829-8c15-56edc54465ea" />
