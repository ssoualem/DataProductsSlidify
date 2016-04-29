---
title       : Visualising US State Facts and Figures with googleVis
subtitle    : For the Developing Data Products course on Coursera
author      :
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Presentation

This Shiny app uses the googleVis package to plot different statistics about US states on a map.

The user can choose what information he wants to see.

The data source is the "state" dataset from R.

The app can be found here : https://ssoualem.shinyapps.io/DataProductsShiny/

--- .class #id  

## Available statistics for each state

* Population: Population estimate as of July 1, 1975 (in thousands)

* Income: Per capita income (1974)

* Illiteracy: Illiteracy rate (1970, percent of population)

* Life Expectancy: Life expectancy in years (1969–71)

* Murder rate: Murder and non-negligent manslaughter rate per 100,000 population (1976)

* High-school graduation rate: Percent high-school graduates (1970)

* Number of days below freezing: Mean number of days with minimum temperature below freezing (1931–1960) in capital or large city

* Area: Land area in square miles


--- .class #id  

## Data sample


Source data sample

```r
data(state)
head(state.x77, 4)
```

```
##          Population Income Illiteracy Life Exp Murder HS Grad Frost   Area
## Alabama        3615   3624        2.1    69.05   15.1    41.3    20  50708
## Alaska          365   6315        1.5    69.31   11.3    66.7   152 566432
## Arizona        2212   4530        1.8    70.55    7.8    58.1    15 113417
## Arkansas       2110   3378        1.9    70.66   10.1    39.9    65  51945
```

--- .class #id  

## Demonstration
<img src="assets/img/full_map.png" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" width="920" />

Some information about the data is available in the sidebar.

The precise figure can be seen by hovering the mouse over a state.
