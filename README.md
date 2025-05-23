Landslide Risk Assessment Using Multi-Source Geospatial Data

Project Overview
This project aims to assess landslide risk in vulnerable regions by integrating diverse geospatial datasets including satellite imagery (Landsat, Sentinel-1), elevation models, rainfall records, land cover data, and historical landslide events. The analysis supports early warning systems and disaster risk mitigation efforts by identifying high-risk zones using spatial analysis and machine learning.
Data Sources and Structure
Data Used:
Landsat 8 Surface Reflectance and Thermal Imagery
Sentinel-1 Synthetic Aperture Radar (SAR)
Digital Elevation Model (DEM - SRTM)
Soil and Land Use/Land Cover (LULC) Data
Rainfall and Meteorological Data
Historical Landslide Event Records
OpenStreetMap (OSM) Infrastructure Layers
Repository Structure:
Landsat/
└── 01042024/
├── (TIF files: spectral bands and thermal data)
Scripts/
├── preprocessing.ipynb
├── risk_model.py
.gitattributes (for Git LFS tracked files)
README.md

Note: Large .TIF files are tracked using Git LFS due to size constraints.

Installation and Setup
To reproduce the analysis:
Requirements:

Python version 3.8 or higher
Python packages: rasterio, numpy, pandas, matplotlib, scikit-learn, geopandas
Setup Instructions:

Clone the repository:
git clone https://github.com/SOHAM240104/landslide-risk-assessment-.git
cd landslide-risk-assessment-
Install Git LFS and dependencies:
git lfs install
pip install -r requirements.txt
Optional Tools:

QGIS for visual inspection
Jupyter Notebook for interactive analysis
Usage
Step 1: Preprocess Data
Run preprocessing.ipynb to clean and extract terrain, vegetation, and water indices.
Step 2: Run Risk Model
Use risk_model.py to generate a risk map using weighted overlay or machine learning classifiers.

Step 3: Visualize Output
Export GeoTIFFs or shapefiles to view in QGIS or web-based tools.

Credits and References
Developed by: Soham
Institution: Anna University (IT Purple Tag)
Key References:

USGS Landsat Data (https://landsat.usgs.gov)
Sentinel Hub (https://www.sentinel-hub.com/)
Git LFS Documentation (https://git-lfs.github.com)
