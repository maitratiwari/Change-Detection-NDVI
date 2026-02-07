# 🌿 Mumbai NDVI Change Detection (Google Earth Engine)

## 🔗 Live App
Explore it here: [Mumbai NDVI Change Detection](https://maitratiwari.users.earthengine.app/view/change-detection-ndvi)

---

## 📍 Overview
This project performs vegetation change detection over Mumbai using Sentinel-2 surface reflectance imagery in Google Earth Engine (GEE). NDVI values from two selected years and a chosen month are compared to identify vegetation **gain**, **loss**, and **stable** regions.

---

## 🗺️ Study Area
The analysis covers Mumbai administrative regions (Mumbai, Mumbai City, Mumbai Suburban, and Greater Mumbai), merged into a single study boundary for processing.

---

## ⚙️ Method Summary
The workflow includes:

- Sentinel-2 filtering by region, date, and cloud coverage  
- Cloud and cirrus masking using QA60 band  
- Reflectance scaling and median compositing  
- Water masking using NDWI  
- NDVI computation and masking of non-vegetation (NDVI < 0.2)  
- NDVI differencing between two time periods  
- Classification into vegetation gain, loss, and stable zones  
- Histogram generation for NDVI change distribution
- Export of change results as polygon shapefiles

---

## 📊 Interface & Outputs
A Google Earth Engine interface allows selection of start year, end year, and analysis month (March or October), and runs the workflow interactively.

Outputs include:
- NDVI change visualization
- Vegetation gain, loss, and stable layers
- NDVI change histogram
- Shape files

---

## ▶️ Usage
Open the provided **GEE application link** or run the script in the Google Earth Engine Code Editor, select the desired years and month, and execute the workflow to visualize results.

