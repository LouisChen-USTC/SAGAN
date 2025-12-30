# SAGAN
_SAGAN is short for Spectral Analysis of Galaxy and Active galactic Nuclei_

The models are based on and fully compatible with [Astropy.modeling](https://docs.astropy.org/en/stable/modeling/index.html).

Please refer to the demo jupyter notebooks in the `example` folder to use the code.

Exponential Gaussian emission profiles and absorption models using P-Cygni profiles as well as pure Gaussian optical depth profiles added. Support forward modeling given the sigma of the LSF (Credited to Shangguan). The P-Cygni profile is modified based on https://github.com/unoebauer/public-astro-tools for the Elementary-Supernova model. Note that the calculation currently is EXTREMELY slow and is almost impossible to use P-Cygni profile for MCMC, or even LesMardt optimizer. Users are adviced to first interpolate on a pre-calculated grid for the absorption P-Cygni spectra.
