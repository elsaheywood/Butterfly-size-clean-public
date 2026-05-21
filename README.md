# Butterfly-size-clean
This repository contains code, data and figures to support Heywood et al. *Museum specimens reveal butterfly size increases through time but divergent responses to temperature*

# Structure:

`src/` Contains R scripts (.rmd markdown format) to reproduce all results and figures. Scripts are numbered for the order they would need to be run.

- `Cleaning1.rmd`: Data assimilation and initial filtering of NHM data, includes links to original data sources.
- `Cleaning2.rmd`: Data assimilation, location name cleaning and initial filtering of OUMNH data.
- `Cleaning3.rmd`: GIS wrangling of temperature data. Includes links to original data sources.
- `Cleaning4.rmd`: Calculation of location coordinates from areas in the Oxford dataset.
- `Cleaning5.rmd`: Tackling brood labeling and matching temperature data to species late-larval period.
- `StatsFitting1.rmd`: Fitting species-level models (Size~ Year+Temp+ Lat+Sex) for both datasets, and comparing model fits with and without a spatial autocorrelation term.  
- `StatsFitting2.rmd`: Across-species models for NHM dataset (two versions, with and without spatial autocorrelation terms for comparison)
- `StatsFitting3.rmd`: Across-species models for Oxford dataset, and comparison between the two museum datasets.
- `StatsFitting4.rmd`: Plots of species trait correlations.
- `StatsFitting5.rmd`: Investigating value of fitting separate coefficients for each sex. 
- `SuppInfo1.rmd`: Makes table of species details.
- `SuppInfo2.rmd`: Makes maps and plots of distribution of data for each species.
- `SI.tex` compiles the pdf for the SI files.

Package details are available in `sessionInfo()` at the bottom of each corresponding .html.

`data/` Contains raw and semi-processed data. (Navigating these files would be easiest from the respective R scripts described above).

`figs/` Contains output figures.

`NHM_modelfitsM1/` Contains species level model fits (brms) for the NHM data.

`NHM_modelfitsSpatial/` Contains species level model fits (brms) for the NHM data including the spatial autocorrelation terms. 

`OUM_modelfitsM1/` Contains species level model fits (brms) for the Oxford data.

`OUM_modelfitsSpatial/` Contains species level model fits (brms) for the Oxford data including the spatial autocorrelation terms. .

`TopLevelModelFits/` Contains top-level (cross-species) model fits (brms).

`statsresults/` Contains `.csv` files of the posterior summaries and LOO comparisons.

# Data Re-use Note:

Processed, public, datasets from other authors (Wilson et al https://doi.org/10.1111/2041-210X.13844, Paterson et al. https://doi.org/10.5519/0038559, Met Office) are included in this repository for ease of reproduction. Any future use should cite the original sources.

<<<<<<< Updated upstream
All our new code and  new measurements can be re-used under Creative Commons 0, but if relevant please cite the main paper. 
=======
All our new code and new measurements can be re-used under Creative Commons 0, but if relevant please cite the main paper. 
>>>>>>> Stashed changes
