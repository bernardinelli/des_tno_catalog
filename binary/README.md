#### Photometric and astrometric record

These are the columns included in the release. They correspond only to resolved observations - for the unresolved observations see the `fluxes` directory
- `EXPNUM`: DECam exposure number
- `BAND`: band used in the exposure
- `RA`: central right ascension (deg)
- `DEC`: central declination (deg)
- `SEP`: separation between the two components (arcsec)
- `PA`: position angle of the separation vector (radians)
- `COV_PA_SEP`: 2x2 covariance matrix of these two measurements
- `FLUX_PRIMARY/SECONDARY`: flux measurement (with zeropoint = 30) of the primary and secondary sources
- `FLUX_ERR_PRIMARY/SECONDARY`: uncertainty of the flux measurement of the primary and secondary sources
- `MAG_PRIMARY/SECONDARY`: magnitude of the primary/secondary sources
- `MAG_ERR_PRIMARY/SECONDARY`: magnitude uncertainity of the primary/secondary sources
- `t_obs`: observation time (in years after J2000.0, TDB scale)
- `t_light`: light travel corrected observation time (same scale as `t_obs`)
- `FLUX_COV`: covariance between the primary and secondary flux measurements

### Orbital solution chains
The orbital solution chains are arrays, where each line has 7 elements, corresponding to:
- Semi-major axis of the orbit (km)
- Eccentricity
- Mutual inclination (radians)
- Argument of perihelion (radians)
- Longitude of ascending node (radians)
- Mean anomaly (radians)
- Period of the orbit (days)


These are all measured with respect to the equatorial reference system. 