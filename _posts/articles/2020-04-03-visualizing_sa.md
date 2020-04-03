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

For the past 5 years I have taught an introduction to spatial statistics seminar at the Winter/Summer GIS Institute hosted by Spatial Structures in the Social Sciences (S4) at Brown University. Most of the institute is geared to teaching people with no GIS background how to work with spatial data and make maps using ArcMap.

This is actually a pretty tall order. Nobody signed up to take a spatial statistics course, and usually only a handful of people are even quantitative researcher. This has forced me to think hard about which concepts are most important and find ways to make them accessible for sociologists, economists, and humanities researchers alike.

So for the past institute, I developed a shiny app that simulates some data, and then visualizes spatial autocorrelation using a grid layout and scatterplot. A slide on the left allows the student to control the level of spatial autocorrelation which is then reflected in the values on the two plots. Students (or instructor) can also change the definition of a neighbor by changing the order of contiguity to see how this may impact spatial autocorrelation.

The scatterplot view of the data is particularly useful as a teaching tool the next step is typically to discuss ways to measure spatial autocorrelation. This can get pretty technical but it doesn't have to. The scatterplot shows the actual values of the squares on the x-axis plotted against the average of all the neighboring squares. Adding the regression line makes it very easy to see how changing values of spatial autocorrelation change the relationship between the values in the square even where it isn't obvious on the grid. Furthermore, the scatterplot is conceptually similar to the Moran's I scatterplot which is simply a scaled version of this same plot. As an instructor, the app allows me to easily show what spatial autocorrelation looks like on map (the grid) and what it means for the data, while simplifying the conceptual step to measurement.

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
