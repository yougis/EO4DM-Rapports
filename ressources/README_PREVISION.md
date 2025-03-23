================================================================================
             Vegetation Drought Index Forecast Program (R version)
================================================================================

Author: Alexandre Peltier
Contact: alexandre.peltier@meteo.fr

================================================================================
                               Program Description
================================================================================

This program generates vegetation drought index forecasts for New Caledonia based on rainfall measurements from previous months and Global Drought Observatory (GDO) seasonal forecasts. The forecasts are generated using statistical models implemented in R.

================================================================================
                            Required R Packages
================================================================================

The program requires the following R packages to be installed:

- ncdf4
- tidyr
- dplyr
- forcats
- ordinal
- sp
- gstat
- spacetime
- rgdal
- rgeos
- maps
- mapdata
- mapproj
- maptools
- sf
- curl
- rvest
- rlang

You can install these packages using the `install.packages()` function in R.

================================================================================
                             Useful Functions
================================================================================

The program includes several custom functions for handling data retrieval from FTP servers, data processing, and modeling. These functions are documented within the code.

================================================================================
                          Data Sources and Repositories
================================================================================

- **GDO Data**: Retrieved from the European Commission's Joint Research Centre (JRC) Drought Observatory datasets.
- **OKAPI Data**: Retrieved from the French Meteorological Service (Météo-France) FTP server.
- **Remote Sensing Data (VHI)**: Retrieved from a local repository.
- **Statistical Models**: Ordinal logistic models are used for forecasting drought indices.

================================================================================
                              Input Data Files
================================================================================

The program requires the following input data files:

- **VHI Data**: Monthly Vegetation Health Index (VHI) data for New Caledonia.
- **GDO Data**: Global Drought Observatory (GDO) seasonal forecast data.
- **OKAPI Data**: Standardized Precipitation Index (SPI) data.
- **Communal Contours Shapefile**: Defines the boundaries of municipalities in New Caledonia.
- **Mask File**: Used for calculating the remote sensing index.

================================================================================
                              Output Data Files
================================================================================

The program generates the following output data files:

- **Model Inputs**: CSV file containing input data for statistical models.
- **Forecast Probabilities**: CSV file containing forecast probabilities.
- **Vegetation Indices**: CSV file containing vegetation drought indices.
- **Rainfall Indices**: CSV file containing rainfall indices.

================================================================================
                               How to Run the Program
================================================================================

1. Ensure that all required R packages are installed.
2. Make sure that the necessary input data files are available.
3. Run the R script "Vegetation_Drought_Index_Forecast.R".

================================================================================
                                  Disclaimer
================================================================================

This program is provided as-is, without any warranty, expressed or implied. The author is not responsible for any damages or losses arising from the use of this program.

================================================================================
