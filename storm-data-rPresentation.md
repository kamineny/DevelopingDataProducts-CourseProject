Developing Data Products - Course Project
========================================================
author: Sridher Kaminani
date: Sun Feb 22 15:04:17 2015


Storm Data Explorer
========================================================
type: sub-section

This presentation is created for the peer assessment for the coursera Developing Data Products class. 

The assignment is geared toward ensuring the following concepts were well understood by the students

- **shiny** to build data product application
- **R-Presentation or slidify** to create data product related presentations


The Application
========================================================
type: sub-section
The purpose of this application is to display the understanding of using **shiny** to build a simple application called **Storm Data Explorer**. This has been developed and deployed at: 
https://kamineny.shinyapps.io/storm-data/

The application allows the user to:
- Select the inputs such as the range of years, types of weather related events. 
- Select the format of the output to be displayed on the map, or as a graph, or as a table and option to download the filtered data.

The Data
========================================================
type: sub-section
This application is based on the U.S. National Oceanic and Atmospheric Administration's (NOAA) storm database.

Dataset has been obtained from [here](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2) and processed for the course project. This is the same file we used for the Cousera's Reproducible Research Course.

Source code for the project is available on the [GitHub](https://github.com/kamineny/DevelopingDataProducts-CourseProject).


Data
=====================
type: sub-section
Sample Data

```r
library(data.table)
dt <- fread('data\\events.agg.csv')
head(dt)
```

```
   YEAR   STATE  EVTYPE COUNT FATALITIES INJURIES PROPDMG CROPDMG
1: 1950 alabama TORNADO     2          0       15 0.02750       0
2: 1951 alabama TORNADO     5          0       13 0.03500       0
3: 1952 alabama TORNADO    13          6      116 5.45250       0
4: 1953 alabama TORNADO    22         16      248 3.07000       0
5: 1954 alabama TORNADO    10          0       36 0.60753       0
6: 1955 alabama TORNADO     8          5       27 7.58000       0
```
