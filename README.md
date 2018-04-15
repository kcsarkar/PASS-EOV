# PASS-EOV
This is Projection Analysis Software for Simulations. version Edge On View
Writer: Kartick C Sarkar
Last updated: 15.04.2018
Compatible code: PLUTO

In astrophysics we often perform (magneto) hydrodynamical simulations to understand the fluid flow in different systems.
Theses simulations can be one, two or three dimnsional in nature. The objective of these simulations is, sometimes, to estimate
the observables as we would see them. Unfortunately, for the astronomical objects we always see a projected map on the sky rather than the whole 3D structure. 

PASS helps to project the simulated data on the sky plane by integrating the line of sight somponent of the simulation box. 
It does not matter if the simulation is 1D/2D/3D, PASS can project it. It assumes simple spherical symmetry for 1D, axisymmetry
around the rotation axis for 2D simulations to project the data. The EOV version integrates the ibservables along the x-axis and projects the result on the Y-Z plane. If you have simulated a case for our Milky-Way Galaxy, and want to project it on Solar Position View, pleas see PASS-SPV.

By default, PASS has options to calculate 
i) total column density
ii) Emission measure in any given temperature range
iii) X-ray surface brightness for electron-proton plasma
iv) X-ray surface brightness including metal contribution from free-free and free-bound mechanisms assuming APEC/Mekal/RS emission models. It can also generate detailed X-ray spectra with an energy resolution of 0.002 KeV.

PASS currently supports the binary datafiles generated from PLUTO (mignone etal, 2007) 1D/2D/3D Spherical/Cylindrical/cartesian simulations.

Let's hope for the best.
