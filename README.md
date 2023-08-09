This repository contains the full data release for the 814 outer Solar System objects found in the Dark Energy Survey.

A full description of the object search is described in [Bernardinelli et al (2022)](https://ui.adsabs.harvard.edu/abs/2022ApJS..258...41B/abstract), and a full description of the photometric processing is described in [Bernardinelli et al (2023)](https://ui.adsabs.harvard.edu/abs/2023arXiv230403017B/abstract). If you use these files, we ask you to cite the corresponding papers.

The FITS table `y6_des_tnos_color.fits` contains both the orbital elements and the colors for each object. The full description of the orbital element information is given in Table 3 of [Bernardinelli et al (2022)](https://ui.adsabs.harvard.edu/abs/2022ApJS..258...41B/abstract). In addition to these, the table also includes the mean absolute magnitudes in each band, as well as mean $(g-r,r-i,r-z)$ colors and their corresponding covariance matrix, and the 68% confidence interval for the lightcurve amplitude.

Inside the `fluxes` directory, the complete photometric record for each object is included in a `hdf5` file (for each object), and the MCMC chains for their fluxes and LCAs. The three Jupyter Notebooks included in the `notebooks` directory explains the columns and how to use these files to reproduce the results of the paper. Inside this directory there are also additional files needed to reproduce the code.

The `binary` directory has the MCMC chains for their mutual orbits (in `.npy` files), as well as the astrometric and photometric record for the binary measurements. Another `README` file is included in that directory with a detailed explanation.
