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

# ---------------------------------------------------------

### Additional support in PASS-1.1 compared to PASS-1.0
### Changes completed on 03rd March 2017

    1. Cartesian coordinates
    2. Autodetects negative Y/Z ranges and start computation accordingly
    3. Can work with multiple files (need to mention in the GUI or head.h)
    4. Does not load additional variables into RAM thus expanding opportunity to
    work with high resolution 3D data.

 Technical Changes
 
    1. Changed data structure from 1D array to a structure of variables so that 
      individual variables can be loaded independently.
    2. The mentioned number of projection grids now accommodate the whole range
    (unlike EOV-1.0 where this grid would cover only the positive quadrant)
    3. The python GUI has been upgraded to work with new PLUTO versions  


###
###  Changes from pass-1.1 to pass-1.2
###  Completed on 23rd March 2017

    1. The major upgradation of this version is to incorporate a viewing angle
       in pass. The new version of pass can rotate the data around Y-axis of 
	PLUTO. The code now requires input THETA which is the angle between 
	PLUTO X-axis and the .
    2. The data type of the input files have to be mentioned now in the GUI/head.h.
	This chage has been incorporated to work with both float and double
	precision data. While float is more suitable for saving large 3D datasets,
	double may be preferred to save high precision data.

  Technical changes

    1. No major upgradation

 
###
### Changes from pass 1.2 to 1.4
### Completed on 15th April, 2018

    1. Added support for APEC and RS plasma models

   Technical changes:
	
     1. Nothing major.
