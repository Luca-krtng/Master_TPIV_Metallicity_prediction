Stellar Photometry and Calibration Project

This repository contains a collection of Jupyter Notebooks and data files focused on stellar parameter visualization, flux calculations, and the creation of calibration plans for MS (Main Sequence) and RG (Red Giant) stars using various survey data including SDSS, PS1 and Euclid.

Project Overview
The project involves several key analysis steps:

Visualizing stellar parameters using the AMBRE synthetic dataset.

Calculating fluxes and magnitudes for pseudo color-color diagrams.

Developing calibration plans for stellar selection based on luminosity.

Comparing observed data against theoretical isochrones and literature such as Starkenburg et al. (2017).

File Structure
Jupyter Notebooks
plot-stellar-param.ipynb: File used to visualise stellar parameters from the AMBRE synthetic dataset.

Starkenburg_paper-diagram.ipynb: File that reproduces the plot from Starkenburg et al. (2017) regarding pseudo color-color diagrams for PS1 and g-i color.

different-surveyv2.ipynb: File that plots pseudo color-color diagrams for g-i and g-r for PS1 and SDSS, as well as Gaia (BP-RP) color.

Euclid-photometry.ipynb: File (along with saved fluxes and magnitudes) for the pseudo color-color diagram for Euclid photometry.

Luminosity-determination.ipynb: File that plots and selects MS and RG stars with isochrones and then plots pseudo color-color diagrams with a polynomial fit.

Calibration-plan.ipynb: File that creates the calibration plans for MS and RG stars using the saved polynomial fit.

Observation-determination.ipynb: File that overlays the training sample on the calibration plan and plots error statistics.

PS1-invistigation.ipynb: File used to see the separability of log(g).

Data and Supplementary Files
observed-data.zip: Observed data considered (using only the training sample).

isochrones.zip: Isochrones considered for the selection of the stars for the calibration plan.

filter.zip: Filters used for the flux calculation, also available for SDSS, PS1, Gaia, and Euclid.

Euclid_magnitude.parquet: Saved fluxes and magnitudes for Euclid photometry.

calculated_magnitudes.parquet: Saved data used to avoid recalculating flux for PS1 and SDSS.

calibration_grids.npz.zip: Compressed file containing calibration grids.

External Resources
The filters used for flux calculations in this project can be found at the Spanish Virtual Observatory (SVO) Theory Filter Profile Service:
https://svo2.cab.inta-csic.es/theory/fps/index.php?mode=browse&gname=PAN-STARRS&asttype=
