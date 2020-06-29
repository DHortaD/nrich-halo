# nrich-halo

This repository contains code which will allow you to replicate the results presented in the paper 'The contribution of N-rich stars to the Galactic Stellar halo using APOGEE red giants' (Horta et al. 2020c). 

# Dependencies

In order to run this code you will need numpy, astropy, tqdm, matplotlib, and scipy installed. You will also need to have a working installation of emcee for performing MCMC.

Next up, you will have to download the custom low metallicity PARSEC isochrone grid used for this paper. If these files are no longer available, you will have to generate a new set of isochrones between Z = 0.0001 and 0.0030 with Delta_Z = 0.0001 from the CMD interface. This grid should then be placed in a logical place, and the environment variable ISODIST_DATA set pointing to this location. ISODIST_DATA is the environment variable used for locating isochrones in the isodist package, in case you already use that. Note however, that this package is not required explicitly for running the code.

# Results:

- Compute the APOGEE DR16 selection function
- Fit the density of APOGEE red giants in the halo, and the N-rich star counterparts
- Perform an estimation of the ratio of N-rich stars to the halo field
- Estimate the mass within a halo/N-rich star sample within a chosen volume

