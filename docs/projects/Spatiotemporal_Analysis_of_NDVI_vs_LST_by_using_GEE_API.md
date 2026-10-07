# Spatiotemporal Analysis of NDVI and LST Correlation in Batticaloa District, Sri Lanka

![Project overview image](../assets/images/project1-cover.png)

## Overview

A freelance remote sensing project that compares vegetation greenness (NDVI) and Land Surface Temperature (LST) across Batticaloa District for three periods: 2014–2015, 2019–2020 and 2024–2025. Landsat 8 imagery was processed in Google Earth Engine, and the results were mapped in QGIS to show how surface temperature relates to vegetation cover.

**Study Area:** Batticaloa District, Sri Lanka  
**Duration:** 21-June-2026 – 03-July-2026  
**Role:** Solo project (Freelance)  
**Status:** Completed and delivered in schedule

---

## Methods & Tools

**Data Sources**

- USGS Landsat 8 Satellite Imagery, Level 2, Collection 2, Tier 1
- Google Earth Engine Data Catalog

**Processing Steps**

1. Filtered Landsat 8 scenes to Batticaloa District for each study period, restricting the collection to the summer window (15th, July – 15th, August).
2. Applied cloud masking and built a median composite for each period.
3. Calculated NDVI from the near-infrared and red bands.
4. Calculated LST from Band 10 brightness temperature and land surface emissivity derived from NDVI.
5. Exported the results and classified them into five NDVI classes and five LST classes.
6. Produced the layouts and maps in QGIS, with a consistent legend and scale across all three periods.

**Tools Used**

| Tool | Purpose |
|------|---------|
| Google Earth Engine (API) | Satellite image filtering, cloud masking, NDVI and LST computation |
| QGIS Desktop LTR 3.40.15 | Map layouts, classification and cartographic design |
| Landsat 8 (USGS) | Source imagery for surface reflectance and thermal data |

**Coordinate System**

- Layers are maintained in WGS 84 / UTM Zone 44N
- Grid coordinates are shown in WGS 84 (decimal degrees)

---

## Key Findings

- LST across the district ranged from roughly 37 °C to 47 °C during the summer window.
- NDVI and LST show an inverse relationship: areas with dense vegetation are cooler, while sparsely vegetated and bare areas record the highest temperatures.
- Side-by-side maps for 2014–2015, 2019–2020 and 2024–2025 make it possible to compare how this pattern has changed over a decade.

---

## Links

[View Code on GitHub](https://github.com/rifasrafeek/Project_Source_Codes/blob/ef7df57e6b057bae4c44b326facaacb661cc36d7/LST_NDVI_GEE_Source_Code){ .md-button }
[View Code in Google Earth Engine](https://code.earthengine.google.com/69cfe6bfc204e53f705f804aeccc41b4){ .md-button }
[View Data Source](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_L2){ .md-button }