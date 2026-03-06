# cloud_computing
Final assignment

# Landsat Timeseries Analysis for the Central Peruvian Rainforest

by Jolien Grafe
Matrikelnr. 3296310
Course: Cloud Computing in Remote Sensing (WS 2025/2026)

In the tropical rainforest of central Peru, deforestation is progressing rapidly. In need of more land for cultivation of in this case pineapple and cafe, farmers burn down rainforest every year, "climbing" higher and higher into the mountains. First, they settled near the river, now they are using fields in areas with high inclination. 
So the idea of this analysis was to demonstrate this development analyzing Landsat NDVI time series. Therefor I defined an AOI near the city of Pichanqui in Chanchamayo, Peru. 

The actual analysis and code with explanations is provided in the Jupyter Notebook, which I attached as well. It is also  To reproduce the code below you will need:
-	a google earth engine account and the python API
-	all the packages mentioned in the import section installed in your environment
-	the notebook saved on your local machine, part 3 will create the folder "exports_no_forest" and download aprox. 100 KB of data and save it there. 

The notebook is divided in three parts:
1.	NDVI timeseries analysis per decade, using L5, L7, L8 and L9 images
2.	NDVI timeseries analysis per 5 year periode, only using L7
3.	Timestep Map showing the deforestation per 5-year period
The final result is this timestep map, which should be the final output of the Jupyter Notebook:

<img width="496" height="374" alt="image" src="https://github.com/user-attachments/assets/e7700111-0e5e-41a9-b24d-c8ea8d1ab15f" />

# Discussion and conclusion
On the map you can see the city center, the rivers and the expanding deforestation. The blue areas have been no-forest areas since the beginning of the century and then there are new parcels of no-forest area for every 5-year period. The fields are pretty small and of different shapes and most of the times areas close to each other correspond to consecutive time-periods. That could be interpreted in a way, that the farmers first work on one parcel, and then extend it step by step or more people start to use the land in the area. The terrain further away from the river rapidly starts to become steeper and therefor more difficult to work on, but the need of more land for plantations drives the people into those terrains. So the observed pattern coincides with the expected development, even though there are some debilities concerning the method.

The use of optical data always comes with the problem of cloud cover, especially in tropical regions. I tried more remote areas, "up the mountain" but there are not very many cloudfree pixels. Therefor I chose an AOI in the lower region, with less cloud cover. 

The thresholds applied can also be discussed, the small-scale changes of coffee plantations (sometimes even with trees for shadow), regrowth-areas and remaining forest are quite challenging. For a further analysis, ground truth data should be considered, since it is also difficult to distinguish those classes in the optical landsat images, because of the coarse resolution. 
 
Also, the described problem with the different sensors, that partly could not even be explained by myself, result in a shorter timeseries. So in order to use this approach in different areas and on greater scales, it would definitely need some refinement. Especially for longer time series, because you would want to use different Landsat Sensors, not only L7 like I did. The harmonized Sentinel and Landsat data set could be an option, as well as the use SAR-data instead of optical, VH-polarized data could also be used to detect deforestation for example. 
