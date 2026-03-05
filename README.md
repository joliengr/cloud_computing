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
