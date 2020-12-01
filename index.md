# Global Precipitation Climatology Project (GPCP) & Mid-Latitude Seasonal Ocsilation (MLSO)
## *Zak Manthos*
***
### The Question:
The main scientific topic I want to explore is precipitation variability. Precipitation and other weather phenomena vary for many reasons which vary in scale from meters to tens of thousand of kilometers and from minutes to decades. Trying to understand the reasons why precipitation does what it does is a complex set of questions that if answered could have major societal benfits.

In much of the analyses completed I try to connect the dots, if any, between precipitation and the Mid-Latitude Seasonal Oscillation (MLSO). It is well documented that there are large scale teleconnections, like ENSO, that have can influence precipitation over large areas and timescales. The MSLO is akin to the larger teleconnections and oscillation, it is a mode of variability for the Northern Hemisphere. It has an average period of 120 days. The MLSO has phases that lineup closely with the North Atlantic Oscillation (NAO) and the Pacific North American pattern (PNA), both of which have been shown to cause precipitation variability across North America.

The El Nino Southern Oscillation (ENSO) index is also used for a comparison.

***

### The Datasets:
**GPCP Dataset:**

The GPCP dataset is a one degree by one degree daily dataset that covers the time span of 1996-10-01 to 2020-05-31. This dataset is derived from satelite data. The dataset has been shown to match up well with reanalyses and ground measurements for the daily precipitation values. 

For more info: [Global-Precipitation-at-One-Degree-Daily](https://journals.ametsoc.org/jhm/article/2/1/36/4943/Global-Precipitation-at-One-Degree-Daily)
    
 - Location: /scratch/zmanthos/GPCP/
 - Files: gpcp_v01r03_daily.2020.nc  Yearly with Daily data
 - Date Range: 1996-10-01 to 2020-05-31
 - Grid resolution: 1x1 degree
 - Source: University of Maryland, Earth Systems Science Interdisciplinary Center
 - *Lots of Metadata stored in the files
    
**MLSO Index:**

The MLSO is a daily standardize climate index for a mode of variability in the Nothern Hemisphere. The index spans from 1979-01-01 to 2019-08-31.

For more info: [Intra‑seasonal and seasonal variability of the Northern Hemisphere extra‑tropics](https://doi.org/10.1007/s00382-019-04827-9)

 - Location: /data/vortex/scratch/
 - File: mlso.index.01011979-08312019.nc
 - Date Range: 1979-01-01 to 2019-08-31
 - Resolution: Daily
 - Source: George Mason University, Dr Cristiana Stan

**ENSO Index**

This ENSO index is a quasi-daily standardized index for the NINO 3.4 region. It is quasi daily because the dataset used, NOAA Optimum Interpolation (OI) Sea Surface Temperature (SST) V2, is weekly data. The OISSTv2 data used gives a weekly NINO 3.4 index that is then projected onto a daily time series. This leads to a daily index but all seven days of a given week have the same values for the index. This Index spans from 1997-01-01 to 2018-12-31 and only used SST data from that time period.

 - Location: /homes/zmanthos/thesis/index/
 - File: enso.nin34.97-18.nc
 - Date Range: 1997-01-01 to 2018-12-31
 - Resolution: Daily
 - Source: George Mason Univeristy, Zak Manthos


### The Analysis:

#### *Climatology*

First things first, below is a multipanel plot of the climatology of the GPCP data, showing each month individually.

![](climatology.png)
