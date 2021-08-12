# Identifying cold blobs with [Ocetrac](https://ocetrac.readthedocs.io/en/latest/)

### What are marine cold spells?
Marine cold spell (MCS) are rare events of unusally cold sea surface temperatures (SSTs). Unlike [*marine heatwaves*](https://github.com/ocetrac/marine-heatwaves), MCS are believed to benefit marine ecosystem by bringing relief to rising ocean temperatures. However, ocean warming is increasingly making MCS weaker and less frequent (e.g., [Chriswell, 2021](https://www.nature.com/articles/s41467-021-25160-y)). 

### Why do we care about MCS?
Identifying and understanding the mechanisms of MCS may better help us to predict climate refugia for marine species. This will ultimately help us to manage efforts in supporting local aquaculture, marine protected areas, and fishery productivity. 

### How can Ocetrac help?
Ocetrac is a useful tool for identifying and tracking extreme climate anomalies with complex spatiotemporal dynamics. It allows for the characterization of MCS evolution in both time and space. This is critical for understanding MCS as these events are not stationary and can easily move across ocean basins. 

___
## Data Availability
Monthly mean SST from the [NOAA Optimum Interpolation Sea Surface Temperature](https://www.ncdc.noaa.gov/oisst/data-access) (OISST v2.1) dataset are available on the S3 compatible and cloud optimized Object Storage Network and is made acessible through Pangeo-forge. This data is measured from a blend of AVHRR-only satellite and in-situ observations and is available from September 1981 through present on a 1/4º global regular grid.

## Code Availability
The three steps are to (00) preprocess the OISST v2.1 dataset, (01) define extreme temperature values, and (02) identify and track MCS. These steps are broken up into three distinct jupyter notebooks written in python 3. Each notebook saves a single netCDF file (which can be changed to zarr if you're working in the cloud). You should change the path of the save netCDF to your personal directory or clouds storage bucket. 

