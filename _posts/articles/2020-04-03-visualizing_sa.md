---
layout: post
title: "Visualizing Spatial Autocorrelation"
modified:
categories: articles
excerpt:
tags: []
image:
  feature:
date: 2020-04-03T15:21:13+04:00
modified: 2020-04-03T15:21:28+04:00
---

For the past 5 years, I have taught an introduction to spatial statistics seminar at the Winter/Summer GIS Institute hosted by Spatial Structures in the Social Sciences (S4) at Brown University. Most of the institute is geared to teaching people the basics of working with spatial data and make maps using ArcMap.

This is actually a pretty tall order. Nobody signed up to take a spatial statistics course, and usually, only a handful of people are even quantitative researchers. This has forced me to think hard about which concepts are most relevant and find ways to make them accessible for sociologists, economists, and humanities researchers alike.

Spatial autocorrelation is a fundamental concept of spatial statistics. So it is something I spend a lot of time discussing in the seminar. For the past two institutes, I developed a shiny app that simulates some data and then visualizes spatial autocorrelation using a grid and scatterplot. A slider allows students to control the level of spatial autocorrelation, which is then reflected in the values on the two plots (below). Students can also change the order of contiguity to see how defining different spatial weights may impact spatial autocorrelation.

The scatterplot view of the data is particularly useful as a teaching tool because it makes approaches to measuring spatial autocorrelation more intuitive. The scatterplot shows the values of a square (x-axis) plotted against the average of the neighboring squares (y-axis). Adding a regression line makes it easy to see how spatial autocorrelation changes the relationship between values. Furthermore, the scatterplot is conceptually similar to the Moran's I scatterplot, which is simply a scaled version of this same plot. As an instructor, the app allows me to quickly show what spatial autocorrelation looks like on a map (the grid) and what it means for the data while simplifying the conceptual step to measurement.


Code for this can be found at [github](https://github.com/tmarlow/sa_visualization). It is easier to see the on the original page where the layout is respected. See it [HERE](https://thomas-marlow.shinyapps.io/sa_visualization/)

Check it out below and let me know if you have any suggestions!


<div id="Container"
 style="padding-bottom:56.25%; position:relative; display:block; width: 100%">
 <iframe id="saIframe"
  width="100%" height="100%"
  src="https://thomas-marlow.shinyapps.io/sa_visualization/"
  frameborder="0" allowfullscreen=""
  style="position:absolute; top:0; left: 0"></iframe>
</div>
