# Downloading and Plotting River Gauge Data
## Written By Jared Rennie (@jjrennie)

Taps into APIs to get river gauge data and metadata. Two public API's are used. The first is the National Weather Service's <a href='https://water.noaa.gov' target="_blank">National Water Prediction System (NWPS)</a>, and the second is the US Geological Survey's <a href='https://waterdata.usgs.gov/nwis?' target='_blank'>National Water Information System (NWIS)</a>. Note that data in NWPS is only for the last 30 days, so NWIS is also used to get historical data.

- NWPS API Documentation: https://api.water.noaa.gov/nwps/v1/docs/#/Gauges/Gauges_ListGauges
- NWIS API Documentation: https://waterservices.usgs.gov/

### What You Need

First off, the entire codebase works in Python 3. In addition to base Python, you will need the following packages installed: 
- <a href='https://github.com/DOI-USGS/dataretrieval-python' target="_blank">dataretrieval-python</a> (aquire data from nwis)
- pandas and numpy (to slice and dice the data)
- matplotlib and cartopy (to plot the data)
    
The "easiest" way is to install these is by installing <a href='https://www.anaconda.com' target="_blank">anaconda</a>, and then applying <a href='https://conda-forge.org/' target="_blank">conda-forge</a>. Afterward, then you can install the above packages. 

##Launch right now with binder:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jjrennie/river-gauge/HEAD?urlpath=%2Fdoc%2Ftree%2Fnwps-nwis_api.ipynb)
