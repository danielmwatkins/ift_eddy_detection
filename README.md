# ift_eddy_detection
Development and testing of the Lopez-Acosta method for eddy detection in the Greenland Sea.

1. Data. We demonstrate the method with a 2-day case study in the Greenland Sea where the effect of ocean eddies is clearly visible: June 28-29, 2024. The notebook `modis_data_acquisition.ipynb` queries Earthdata, downloads the relevant modules, and then regrids them to a common 250-m resolution. We also need the ERA5 wind data and ORAS5 ocean current estimates.
   * I have working code to access the swath data. There are 32 images available for the 2-day period.
   * I still need to convert the 16-bit integer data to reflectance using the scaling term
   * I need to download the geolocation file, and use that to map the data onto a common grid
   * 
3. Methods. Review the description in Rosalinda's thesis, write it out. Use IFT to segment and track ice floes. Also use ORB to make an estimate ice motion vector field for comparison. 
4. Results. Compare the predicted eddy locations to the images -- are the sizes similar? What can we say about the eddy properties? 
