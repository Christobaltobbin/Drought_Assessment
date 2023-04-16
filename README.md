# Agriculture Drought Assessment of Matongo Region in Tanzania

## Introduction
Drought is one of the natural disasters which has been intensifying over the years due to the effects of climate change and occurs in areas where there is low precipitation or rainfall due to environmental factors. Drought is considered one of the most complex natural hazards because of its slow onset, long-term impact and negatively affecting the lives of people (Zambrano, Lillo-Saavedra, Verbist, & Lagos, 2016). There are four categories of classifying drought according to Willhite and Glantz and these are; Meteorological drought, Hydrological drought, Agricultural drought and Socio-economic drought (Wilhite & Glantz).
Some of the common methods of agriculture drought monitoring is by using indices such as the standardized precipitation index (SPI), Palmer drought severity index (PDSI), and crop moisture index (CMI) but these require the long term record of precipitation data (Shen, et al., 2016). Remote sensing-based indices also include vegetation health index (VHI), temperature condition index (TCI) and vegetation cover indices (Zambrano, Lillo-Saavedra, Verbist, & Lagos, 2016). For this paper, the vegetation condition index (VCI) which is derived from the difference between the maximum and minimum normalized difference vegetation index (NDVI) values.

## Study area
Matongo is located in the northern parts of Tanzania, in the Kilimanjaro region and lies between latitude 3.2806° S and  longitude of 37.1958° E. The region has a hilly landscape with elevations ranging from 600 to 1800m above sea level. Matongo falls within the tropical climate with raining  seasons from March to May and between October and December. Matongo is known for its agriculture with crops such as coffee, maize, beans, and bananas being cultivated. In addition to agriculture, the Matongo region is also home to several tourist attractions, including the Kilimanjaro National Park and the Marangu Waterfalls.
Overall, the Matongo region is an important agricultural area in Tanzania, with a favorable climate and fertile soil supporting the production of high-quality crops. Its location near Mount Kilimanjaro also makes it an important tourist destination, contributing to the local economy. The land cover map of Matongo indicates that most of the region is covered by forest and is followed by agriculture and shrubland.
<p align="center">
  <img src="https://user-images.githubusercontent.com/116877317/232340261-6e9928fc-40f3-4bad-940a-81e29a77a33e.png" align="middle" width="248" height="357">
</p>

## Data
Landsat imagery is one of the most important source of remote sensing satellite data and has been used in several studies and disciplines across the globe.  The Landsat satellite program has been providing high-quality, multispectral remote sensing data for over 40 years (Wulder, Masek, Cohen, Loveland, & Woodcock).
Landsat imagery is multispectral which enables it to captures information in multiple spectral bands. The Landsat sensors capture data in seven spectral bands, ranging from the visible to the thermal infrared (Wulder, Masek, Cohen, Loveland, & Woodcock). In this paper, we would use these multispectral information to analyse drought through the  VCI.

## Method
Landsat 7 images for the years 2002, 2008, 2014 and 2020 within the raining season which is from March to May. All the processing was done in QGIS, also making use of the Semi-automatic classification plugin (SCP) available in  qgis.
The NDVI for each year was calculated using the NDVI formula and also generate the maximum and minimum NDVIs using the cell statistic function in qgis.
                NDVI  = ((NIR-RED) )/( ( NIR+RED)),
Where NIR and Red are the Near infra-red and red bands respectively.
The VCI is also then calculated for from the NDVI. VCI compares the NDVI of  a particular year to that of NDVI values observed within the same period of other years. It is expressed as:
 
VC I(i,p,j)=((NDV I(i,p,j)- NDV I(min))/(NDV I(max)-NDV I(min)))*100

Where ´i´ is for pixel, ´p´ for period and ´y´ the year respectively. For this study, the VCI is expressed as a percentage ranging from extreme drought to no-drought.

## Results
From the VCI maps, the disparity of drought intensity percentages in Matongo for the years 2002, 2008, 2014 and 2020 is illustrated in figure below. The Matongo region reached the lowest percentage of VCI and thus experienced an extreme drought in 2008 (0-10%) and the highest VCI in 2014(75%). The years 2002 exhibited moderate and severe drought while 2020 light to no droughts.

<p align="center">
  <img src="https://user-images.githubusercontent.com/116877317/232346024-ff62205b-fd4c-4da1-8b7d-99a7e9e65720.png" align="middle" width="248" height="350">
</p>

## Conclusion
This study assessed the agriculture drought in the Matongo region of Tanzania using Landsat imagery and the vegetation condition index (VCI). The VCI was derived from the difference between the maximum and minimum NDVI values and the NDVI values for the respective years. The results showed that the Matongo region experienced severe droughts in 2002 and  2008 with a VCI range of 0-20%, while 2014 had the highest VCI range of 75%. This study highlights the importance of remote sensing-based indices in monitoring drought conditions in agricultural areas, especially in regions vulnerable to climate change and by doing so, drought or conditions leading to drought can be detected and adequate measures can be triggered to mitigate the drought and its negative impacts.

##References
Shen, Q., Liang, L., Qian, X., Sun, Q., Zhang, L., Liu, Z., . . . Qin, Z. (2016). Drought trends based on the VCI and its correlation with climate factors in the agricultural areas of China from 1982 to 2010. Environ Monit Assess.
Wilhite, D. A., & Glantz, M. H. (n.d.). Understanding: the Drought Phenomenon: The. Water International.
Wulder, M. A., Masek, J. G., Cohen, W. B., Loveland, T. R., & Woodcock, C. E. (n.d.). Opening the archive: How free data has enabled the science and monitoring promise of Landsat. Remote Sensing of the Environment.
Zambrano, F., Lillo-Saavedra, M., Verbist, K., & Lagos, O. (2016). Sixteen Years of Agricultural Drought Assessment of the BioBío Region in Chile Using a 250 m Resolution Vegetation Condition Index (VCI). Remote Sensing, 20.

