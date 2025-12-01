# Aquaculture Area Portfolio Item :ledger:

## Purpose:

In this assignment for UCSB's Environmental Data Science Geospatial Analysis class, we are investigating the area of suitable habitat for different marine species of aquaculture interest off the West Coast of the USA. We are practicing and demonstrating our skills in raster manipulation, raster math, data visualization, and building and using generalizable workflows within a single R function. This differs from my repository "aquaculture-area-analysis", as it is formatted as a science communication post to add to my portfolio on my website. The analysis is similar, but comminicated and described in a larger scientific context.

## Description:

We are using **Sea Surface Temperature (sst)** and **Bathymetry** data from the ocean off the West Coast of the USA to calculate the suitable habitat in each of the exclusive economic zones in the area for different marine species of aquaculture interest. First, we are masking the temperature and depth data to places that are suitable for a specific species, using data from **SeaLifeBase** to gather the minimum and maximum temperature and depth the species can survive at. Then, we use the **exclusive economic zone** data to calculate the suitable area for the species in each of the zones in order to compare across zones. Last, we are visualizing each zone by the area of suitable habitat for a target species in a map. This workflow is developed step-by-step for oysters, then is built into a single R function for a generalizable workflow that can intake any marine species in this geographic area, given data on the temperature and depth range. This can be used my aquaculture managers to compare and contrast which eez areas are better for which species. 

## Data access:

### SST

Note: this data is in my .gitignore, so it is not available in the repository. However, it was generated from the NOAA Coral Reef Watch 5km Daily Global Satellite Sea Surface Temperature Anomaly, version 3.1, for the years 2008-2012.

### Bathymetry

Note: this data is in my .gitignore, so it is not available in the repository. This data was obtained using General Bathymetric Chart of the Oceans (GEBCO), for the area west of the USA

### Exclusive Economic Zones (EEZ)

Note: this data is in my .gitignore, so it is not available in the repository. This data was obtained Marineregions.org.

### Species thermal and depth tolerance data: SeaLifeBase

Note: this data is in workflow, not imported as data, as I typed in the relevant values throughout the workflow. Data was accessed using SeaLifeBase.

## Authors and contributors

I am the sole author and contributor to this homework assignment. The assignment was written by Ruth Oliver.

## References

### Data citations

### SST

NOAA Coral Reef Watch. NOAA Coral Reef Watch Version 3.1 Daily 5km Satellite Regional Virtual Station Time Series Data for West Coast of USA, 2008 - 2012r. College Park, Maryland, USA: NOAA Coral Reef Watch. Data set accessed at [https://coralreefwatch.noaa.gov/product/vs/data.php](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php).

### Bathymetry

GEBCO Compilation Group (2022) GEBCO_2022 Grid (doi:10.5285/e0f0bb80-ab44-2739-e053-6c86abc0289c).

## EEZ

Flanders Marine Institute (2025): MarineRegions.org. Available online at www.marineregions.org. Consulted on 2025-11-25.

## SeaLifeBase

Palomares, M.L.D. and D. Pauly. Editors. 2025. SeaLifeBase.
World Wide Web electronic publication.
www.sealifebase.org, version (04/2025).

Urchin specific data: https://www.sealifebase.ca/summary/Mesocentrotus-franciscanus.html

Depth tolerance: Lambert, P. and W.C. Austin 2007 Brittle stars, sea urchins and feather stars of British Columbia, Southeast Alaska and Puget Sound. Royal British Columbia Museum, Canada, 150p.

Temperature tolerance: Kaschner, K., K. Kesner-Reyes, C. Garilao, J. Rius-Barile, T. Rees and R. Froese 2016 AquaMaps: predicted range maps for aquatic species. World wide web electronic publication, www.aquamaps.org, Version 08/2016.

# Repository structure

```
├── aquaculture-area-portfolio-item.qmd
├── aquaculture-area-portfolio-item.Rproj
├── data
│   ├── average_annual_sst_2008.tif
│   ├── average_annual_sst_2009.tif
│   ├── average_annual_sst_2010.tif
│   ├── average_annual_sst_2011.tif
│   ├── average_annual_sst_2012.tif
│   ├── depth.tif
│   ├── wc_regions_clean.dbf
│   ├── wc_regions_clean.prj
│   ├── wc_regions_clean.shp
│   └── wc_regions_clean.shx
└── README.md
```
