## Evaluating the Impact of Spatial Resolution and Topography on Climate Model Predictions

This project explores whether topographic information, specifically slope, can help lower-resolution land surface model simulations replicate key outputs typically achieved at higher resolutions. This work was conducted using the Joint UK Land Environment Simulator (JULES), focusing on Exmoor National Park in the UK—a topographically complex region ideal for testing how terrain affects carbon and water fluxes.

## Overview

- **Model Used**: JULES (Joint UK Land Environment Simulator)
- **Study Area**: Exmoor National Park, UK
- **Time Period**: 2040–2049
- **Spatial Resolutions**: 12 km (coarse) vs 1 km (fine)
- **Goal**: Assess whether adding slope to coarse-resolution inputs improves simulation accuracy

## Why Topography?

Topographic features like slope and elevation drive local climate variability, especially in hilly or mountainous regions. These features influence:

- Rainfall patterns
- Soil moisture retention
- Carbon uptake via plant productivity

Despite this, most regional climate models don’t resolve these variations well due to computational limitations.

##  Methods

- **Climate Input**: UK Climate Projections (UKCP18)
- **Downscaling**: Used the [mesoclim](https://github.com/ilyamaclean/mesoclim) package to downscale 12 km outputs from UKCP18 to 1 km
- **Key Variables Analyzed**:
  - Latent heat flux (W/m²)
  - Soil moisture (kg/m²)
  - Evapotranspiration (mm/day)
  - Runoff (mm/day)
  - Gross Primary Productivity (GPP; gC/m²/day)
- **Statistical Tool**: Pearson correlation analysis

## Key Findings

- **Slope ≠ Strong Driver**: Slope had very weak correlations (R² < 0.06) with carbon and water flux variables.
- **Water–Energy Link Confirmed**: Latent heat flux was strongly correlated with:
  - Soil moisture (r = 1.00)
  - Canopy evaporation (r = 0.93)
  - Negative correlation with runoff (r = -0.90)

These results suggest that slope alone may not be enough to replicate high-resolution model behavior at coarse scales—but that hydrological relationships remain strong.



---

_This study was conducted by Emily Cranston, Department of Geography, University of Georgia under the guidance of Dr. Anna Harper, Department of Geography, University of Georgia._
