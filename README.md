# Soil Erosion Mapping with USLE Model and GIS for Narmada Basin.

## Narmada Basin:
The Narmada Basin, located in central India, spans approximately 98,000 square kilometers and is traversed by the Narmada River, which flows about 1,312 kilometers westward into the Arabian Sea. This region features diverse topography, from the Vindhya and Satpura ranges to fertile plains, supporting a variety of ecosystems.

The Narmada River is crucial for millions, providing water for agriculture, drinking, and hydropower. It also sustains numerous communities, including indigenous populations, and is rich in biodiversity. However, the basin faces significant environmental challenges, including deforestation, urbanization, and soil erosion, which threaten its ecological balance and agricultural sustainability. This project aims to address soil erosion in the Narmada Basin, offering insights for effective resource management and conservation.

### Team Members:
1. [Piyush Pandya](https://github.com/Piyushpandya83)
2. [Parth Patel](https://github.com/ParthPatel-4403)
3. [Viraj Hirapara](https://github.com/Viraj-Patel07)

## Introduction:
Soil erosion is a significant environmental issue in the Narmada Basin, impacting agricultural productivity and ecosystem health. This project aims to map soil erosion using the Universal Soil Loss Equation (USLE) and Geographic Information Systems (GIS). By integrating these tools, we can create detailed maps highlighting areas at risk of erosion, which will aid in informed land use and conservation decisions. The study will enhance understanding of erosion patterns, identify critical intervention zones, and promote sustainable land management, ultimately preserving soil resources and supporting local communities.

## Data Sources
* CHIRPS (Climate Hazards Group InfraRed Precipitation with Station Data)
  * Source: UCSB CHG
  * Use: Rainfall data for R Factor calculation.
* OpenLandMap Soil Data
  * Source: OpenLandMap
  * Use: Soil texture classification for K Factor calculation.
* SRTM (Shuttle Radar Topography Mission)
  * Source: USGS
  * Use: Digital Elevation Model (DEM) for LS Factor calculation.
* Sentinel-2 (Copernicus)
  * Source: European Space Agency
  * Use: NDVI data for C Factor calculation.
* MODIS Land Cover Type
  * Source: NASA MODIS
  * Use: Land cover data for P Factor calculation.
* WWF HydroSHEDS
  * Source: WWF
  * Use: Basin boundary data for defining the Area of Interest (AOI).

### Methodology overview:
* **Step 1**: Data Collection and Preprocessing:
  * Import datasets (DEM, Land Use, Rainfall, Soil)
* **Step 2:** Calculation of USLE Factors using GEE:
  * Rainfall Erosivity (R)
  * Soil Erodibility (K)
  * Topographic Factor (LS)
  * Crop Management Factor (C)
  * Conservation Practices Factor (P)
* **Step 3:** Soil Loss Estimation (A):
  * Combine the factors to calculate soil erosion
  * Visualization of erosion risk areas on GEE Map

## Code Snippet - https://code.earthengine.google.com/d338e8bd6e828ebccc5d5a619543b2e3


* Inspiration: https://github.com/sukantjain/
