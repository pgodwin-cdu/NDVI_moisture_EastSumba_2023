# NDVI_moisture_EastSumba_2023

The following is a description of the files within this resource:

**rainfall-bmkg.csv** CSV file containing monthly rainfall totals in mm from the "Umbu Mehang Kunda" Meteorology Station (station number 97340) in Waingapu, East Sumba, Nusa Tenggara Timur, Indonesia. Daily data can be downloaded as csv files one month at a time via the Indonesian Meterorology, Climatology and Geophysics body (BMKG) https://dataonline.bmkg.go.id/ 

**Haharu_district_boundary.zip** This zip file contains the .shp, .shx., .prj, .dbf, .cpg., and .fix files for the Haharu district boundary that was used for extracting district scale MODIS and Landsat 7 data in Google Earth Engine. We created the shapefileby manually drawing the polygon in Google Earth Engine, using the "draw a shape" tool, to exclude ocean from within the district boundary. We have also shared the shapefile here: https://code.earthengine.google.com/?asset=users/pennybgodwin/Haharu_no_ocean. 

**Vegetation_sites.zip** This zip file contains the .shp, .shx., .prj, .dbf, .cpg., and .fix files for the 10 x 1 ha vegetation patches: Napu, Laikaterik, Karaha, Community Well, Wunga Well 1, Wunga Well 2, Mahogany Plantation, Cashew, Regeneration 1 and Regeneration 2. We have also made these available through GEE:<br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Cashew_orchard_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Community_Well_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Karaha_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Laikaterik_Patch_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Napu_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Regeneration_1_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Regeneration_2_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Well_Wunga_1_32751 <br>
https://code.earthengine.google.com/?asset=users/pennybgodwin/Wunga_Well_2_32751 <br>

**clean_L7_data** is the R script used to remove errors from the patch scale NDVI data exported from GEE

**Median_Haharu_L7_NDVI** is the GEE script to create median Landsat 7 NDVI values at the Haharu district scale, using the Haharu shapefile that has been shared here. We downloaded NDVI data from GEE as a .csv file.

**Median_Haharu_MODIS_NDVI** is the GEE script to create median MODIS Terra NDVI values at the Haharu district scale, using the Haharu shapefile that has been shared here. We downloaded NDVI data from GEE as a .csv file.

**MODIS_L7_Haharu_stats** is the R script we used for computing Haharu scale NDVI statistics for MODIS and Landsat 7 timeseries

**NDVI_L7_Haharu.tif** is a .tif file generated in GEE as a composite image of median NDVI values between 2000 and 2018 with a cloud mask applied. This script we used to create this image is here: <br>
https://code.earthengine.google.com/c3118944cf7c27df7b3eb7fcdc4013e7

**CCF_NDVI_Rainfall** is the R Script we used to generate cross correlation values and plots for monthly Landsat 7 NDVI data at the Haharu district scale and monthly rainfall data.

**landcover_classification** is the link to the GEE script for generating the Sentinel derived landcover classification for the Haharu district: <br> https://code.earthengine.google.com/d1d2edb9bdda7c04817b74d3b74f52f0 

**seasonal_NDVI_site_analysis_R** is the R script we used to generate NDVI ranges by site and site type for anomalous wet seasons

