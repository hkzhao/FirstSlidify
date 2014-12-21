---
title       : Simple Shiny Temperature Converter 
subtitle    : For coursera class Developing Data Product
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Temperature Converter

1. Created a temperature converter by using shiny
2. Formula
3. Source Code
4. Publish to shiny server

--- .class #id 

## Formula

Below is the forumla that converts temperature from Celsius to Fahrenheit:


```r
# function
celsiusToFahrenheit <- function(inval) (inval * 9 / 5) + 32
# test it
celsiusToFahrenheit(32)
```

```
## [1] 89.6
```

The forumla that converts temperature from Fahrenheit to Celsius:


```r
# function
fahrenheitToCelsius <- function(inval) (inval - 32) * 5 / 9
# test it
fahrenheitToCelsius(0)
```

```
## [1] -17.78
```

--- .class #id 

## Source Code
1. ui.R defines the display, including inputs, outputs and other controls
2. server.R defines the temperature conversion functions and does the calculation
3. Complete source code an github https://github.com/hkzhao/FirstShiny

--- .class #id 

## Publish to shiny server

Here are the steps to publish it to shiny server:

1. Make sure you have devtools installed in R
2. Install shinyapps: devtools::install_github('rstudio/shinyapps')
3. Create a ShinyApps.io account
4. Configure shinyapps
5. Detailed instruction: http://shiny.rstudio.com/articles/shinyapps.html
6. The finished shiny server path: https://hkshiny.shinyapps.io/project/
