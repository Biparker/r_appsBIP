---
title       : Kruskal Test Demo
subtitle    : 
author      : Bob Parker
job         : Programmer/Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---


## Slide 2

The r_apps shiny project demonstrates the R kruskal test, and boxplot visualization of the test using an R sample data set: 'airquality'.

Kruskal Test in R determines difference in distribution
of two or more sets of numeric data.

It is non-parametric (ie., does ) assume anything about underlying distribution of the data.

---.class #id

## Slide 3
 

---
## Interactive Chart

--{r echo = F, results = 'asis'}
require(rCharts)
require(datasets)
require(rCharts)

airquality= as.data.frame(airquality)
n1 <- boxplot(Ozone ~ Month,data = airquality)

n1$print('chart1')
---

