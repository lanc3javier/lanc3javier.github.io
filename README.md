# <span style="color: #2e7d32;">Lance Javier</span>

## Professional Summary

---

### Field Expertise (Agronomy, Ecology)

 * **On-Farm Conservation Tillage Soybean and Corn Research**
    * **Objective**
    * **Key Methods**
    * **Results**
 * **Ecotoxicology of Microplastics and Copper on Soybeans and Soil**
    * **Objective**
       * Investigated the ecotoxicology of polyethylene terephthalate (PET) microplastics and copper as co-contaminants, and how they influence soybean growth and soil properties.
    * **Key Methods**
      *  Grew soybeans for 1-month in soil contamination (PET and/or copper) treatments, separated roots from shoots, then measured both plant compartments for biomass and copper uptake.
      *  Used a handheld chlorophyll meter to measure soybean stress.
      *  Built a data analysis pipeline in RStudio that featured statistical tests like ANOVA, Bartlett's, Tukey's Honestly Significant Different post-hoc, and Games-Howell post-hoc.  
    * **Results**
       * The soil's high organic matter content kept copper bioavailability low and left total aboveground biomass unaffected. The combination of microplastics and copper significantly reduced photosynthetic efficiency by ~2.0%. The combined PET and copper treatment led to a ~35% increase in soybean root biomass relative to the control and copper-only treatments.

---

### Technological Skills (GIS, Instrumentation)

 * **Field Stratification Using LiDAR and SWIR Bands to Produce Soil Sampling Zones**
    * **Objective**
       * As part of my MSc research, I had to separate farmer fields into zones with differing levels of estimated crop performance. Plots would then be placed within each zone, in which soil and crop sampling would occur.
       * Two remotely sensed estimators of crop success were used:
          * Topographical Wetness Index (TWI): Greater values indicated lower, and wetter, areas with greater flow contribution from upslope positions.
          * Normalized Difference Tillage Index (NDTI): Greater values indicated greater accumulation of crop surface residues.
    * **Key Methods**
       * Data for TWI was extracted from the Government of Ontario's "Digital Raster Acquisition Project Eastern Ontario (DRAPE)" dataset, which was a LiDAR-derived Digital Elevation Model (DEM)
       * Data for NDTI was extracted from EO-Browser's Sentinel-2-LandSat Dataset, which is a multispectral satellite. Only SWIR Bands (B) 11 and 12 were used for this project.
       * TWI was derived from DEM data processed in RStudio and QGIS using the WhiteBoxTools package. The analytical pipeline consisted of 2x2 resolution smoothing, and calculating slope, flow pointers, and specific contributing area.
       * NDTI was calculated as B11-B12/B11+B12.
       * TWI and NDTI were both cropped to the field boundary; resolutions, extent, and CRS of the two indices were aligned; a k-means clustering, or thresholding technique, were used to split the raster into 4 zones with differing levels of TWI and NDTI.
       * Two plots were assigned into each zone using QGIS for a total of 8 plots/field (2 plots/zone; 4 zones). This workflow was repeated for each of the 9 unique fields.
    * **Results**
       * See the below images for photos of this geospatial analysis pipeline.
  
<img src="sampling_zone_2024.png" alt="Scatter plots of zone stratification." style="width: 50%; height: auto;">

Scatter plots of the topographic wetness index (TWI) and normalized difference tillage index (NDTI) for corresponding pixels across fields sampled in 2024, showing their respective cluster classifications. Each field was stratified into four sampling zones (“clusters”) using k-means clustering with four centers. Two plots were placed within each zone for subsequent field sampling. A fixed white circle marks a common reference point across all facets, corresponding to the overall median TWI and NDTI across all fields. Field numbers are located above each facet.

<img src="sampling_zone_f3_1.png" alt="Map of zone stratification." style="width: 25%; height: auto;">

Sampling zones were produced by k-means clustering analysis of pixels with NDTI and TWI values. The red line delineates the field boundary as defined by the farmer collaborator. Bold black contour lines represent 1-m elevation intervals, while dashed contour lines indicate 0.5-m intervals. Contours were derived from a 2-m resolution digital terrain model (DRAPE dataset). Elevation values (m above sea level) are shown in black text adjacent to contour lines. A north arrow and scale bar are included for reference.

---

### Knowledge Transfer and Training (Presentations, Outreach)


---


#### Featured Presentations

* **CSSS-CSA Joint Conference: Soils and Crops; June 2026**
   * My first-ever poster presentation, where I presented some of the overall conclusions of my thesis concerning soil shear strength and temperature as targets for follow-up research trials.

![CSSS-CSA Conference Poster. June 2026.](CSSS-CSA_2026.PNG)

* **MSc Thesis Defense**
   * Screenshots of some slides used during my MSc thesis defense.

   <p align="center">
  <img src="/MSc_Defense_1.PNG" width="48%" alt="Picture 1" />
  <img src="/MSc_Defense_2.PNG" width="48%" alt="Picture 2" />
  <img src="/MSc_Defense_3.PNG" width="48%" alt="Picture 3" />
  <img src="/MSc_Defense_4.PNG" width="48%" alt="Picture 4" />
</p>

* **Eastern Ontario Crop Conference, January 2026**
   * I presented my MSc thesis research on soybean stand establishment in high-residue, conservation tillage systems, and provided farmer recommendations for improving stand and yield

<p align="center">
  <img src="/EOCC_2.PNG" width="48%" alt="Close-up photo of myself (right) and my MSc supervisor, Dr. Joshua Nasielski (left) presenting at the Eastern Ontario Crop Conference in Kemptville, ON, during January 2026." />
  <img src="/EOCC_3.PNG" width="48%" alt="Wide-angle photo of myself (right) and my MSc supervisor, Dr. Joshua Nasielski (left), on stage, presenting at the Eastern Ontario Crop Conference in Kemptville, ON, during January 2026. The audience was full of farmers, agronomists, and researchers." />
</p>




