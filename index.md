---
title       : "Introduction to Data Visualization"
subtitle    : Some dos and don'ts"
author      : Daniel Anderson
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- 
<style>
em {
  font-style: italic
}
</style>

<style>
strong {
  font-weight: bold;
}
</style>



## Remember

* Get R installed: https://cran.r-project.org
* Get RStudio installed: https://www.rstudio.com/products/rstudio/download/

**NOTE:** If you need help with either of the above, please contact me. I'd like everybody to be ready to go **before** we need to use it. Best to get it installed now and make sure it's working so we can troubleshoot if not.

---- .quote

<q> Above all else, show the data

<br>
Edward Tufte

----
## Hypothetical example
* School wants to try out a new reading intervention
* Work with researchers at the UO to design a study
* Kindergarten students who are behind their peers in literacy are selected
* Randomly assign half the students to the intervention, the rest continue with
  "typical" instruction
* Now the study is over - how do we tell if it worked? Visualize it! (and 
  other stuff too)

----
## Barplots
(tried and true)

![plot of chunk barplot](assets/fig/barplot-1.png)

-----
## Boxplots
(tried and true)

![plot of chunk boxplots](assets/fig/boxplots-1.png)

----
## Notched boxplots
(slightly better)

![plot of chunk notched_boxplots](assets/fig/notched_boxplots-1.png)

----
## Stripcharts
Show the data!

![plot of chunk stripchart](assets/fig/stripchart-1.png)

----
## Jittered stripcharts
Show the data!

![plot of chunk jittered_stripchart](assets/fig/jittered_stripchart-1.png)

---
## Combine barplots and jittered stripcharts

![plot of chunk barplot_stripchart](assets/fig/barplot_stripchart-1.png)

----
## Combine boxplots and jittered stripcharts

![plot of chunk boxplot_jitter](assets/fig/boxplot_jitter-1.png)

----
## Best?

![plot of chunk broman_plot](assets/fig/broman_plot-1.png)

----
## Some things to avoid

* 3D plots
* Pie charts
* Dual axes
* Restricted axes
* Unnecessary frills (colors, etc)
	+ Show the data as plainly as possible. Let the data speak!

NOTE: The following 10 slides (and the previous plot) inspired/taken from Karl Broman's presentation on graphs (see [here](https://www.biostat.wisc.edu/~kbroman/presentations/graphs2017.pdf))

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/3d_bar.png width = 500 height = 500>
</div>

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/tube_bar.png width = 500 height = 500>
</div>


--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/cone_bar.png width = 500 height = 500>
</div>

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/orbs.png width = 500 height = 500>
</div>


--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/pie.png width = 500 height = 500>
</div>

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/exploded_pie.png width = 500 height = 500>
</div>


--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/donut.png width = 500 height = 500>
</div>

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/area.png width = 500 height = 500>
</div>

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/double_terrain.png width = 500 height = 500>
</div>

--- &twocol
## Examples

*** =left

<div align = "center">
<img src = assets/img/broman_plot.png width = 500 height = 500>
</div>

*** =right

<div align = "center">
<img src = assets/img/bad_data_vis/terrain.png width = 500 height = 500>
</div>

----
## Some great examples: SEDA
Sean Reardon: https://cepa.stanford.edu/seda/overview

<div align = "center">
<img src = assets/img/seda.png width = 800 height = 600>
</div>

----
## Means by district
<div align = "center">
<img src = assets/img/seda_means.png width = 900 height = 500>
</div>

----
## Average gains by district
<div align = "center">
<img src = assets/img/seda_growth.png width = 900 height = 500>
</div>

----
## Mean scores and SES
<div align = "center">
<img src = assets/img/seda_ses.png width = 900 height = 500>
</div>

----
## Mean scores and SES by Race/Ethniciy
<div align = "center">
<img src = assets/img/seda_ses_race.png width = 900 height = 500>
</div>

---
## Other examples: Visualizing scale
* Space stuff: http://imgur.com/a/lGabv
<br>
* Time: http://www.sciencealert.com/watch-this-3-minute-animation-will-change-your-perception-of-time

----
## Some *ggplot* examples

![plot of chunk mpgEx3](assets/fig/mpgEx3-1.png)

----
## Add an additional aesthetic

![plot of chunk mpgEx4](assets/fig/mpgEx4-1.png)

----
## Add smooth line for each class
# Too busy

![plot of chunk mpgEx5b](assets/fig/mpgEx5b-1.png)

----
## Remove SE

![plot of chunk mpgEx6a](assets/fig/mpgEx6a-1.png)

---- .segue
# Some things to avoid

----
## Truncated axes
<div align = "center">
<img src = assets/img/bad_data_vis/truncated_axes.png width = 900 height = 500>
</div>

----
<div align = "center">
<img src = assets/img/bad_data_vis/truncated_axes2.png width = 900 height = 500>
</div>

----
## Dual axes
<div align = "center">
<img src = assets/img/bad_data_vis/dual_axes.png width = 900 height = 500>
</div>

----
## Scaling issues
<div align = "center">
<img src = assets/img/bad_data_vis/area_size.png width = 900 height = 500>
</div>

----
## Poor binning choices
<div align = "center">
<img src = assets/img/bad_data_vis/poor_binning.png width = 900 height = 500>
</div>

----
## Some general advice
* Consider the purpose of the plot. 
	+ Relation? Scatterplots 
	+ Distribution? Histogram or density plot
	+ Trend? Line plot, scatterplot with smoother, etc.
* How many variables? What type?
	+ One continuous variable: histogram, density plot, or similar
	+ Two continuous: Scatterplot (if you have lots of data, consider binning)
	+ One categorical one continuous: boxplots, violin plots, bar plots
	+ Two categorical variable? Mosaic plot

----
## One continuous variable
# Histogram
![plot of chunk hist](assets/fig/hist-1.png)

----
## One continuous variable
# Density plot
![plot of chunk density](assets/fig/density-1.png)

----
## One continuous variable
# Frequency polygon
![plot of chunk freqpoly](assets/fig/freqpoly-1.png)

----
## Consider overlays
![plot of chunk overlay](assets/fig/overlay-1.png)

----
## Two continuous variables
# Scatterplot

![plot of chunk scatter](assets/fig/scatter-1.png)

----
## Trend
# Line plot (often with date or time on x-axis)
![plot of chunk trend](assets/fig/trend-1.png)

----
## Trend w/smoother

![plot of chunk trend_smooth](assets/fig/trend_smooth-1.png)

---
## Categorical & Continuous
# Violin plots

![plot of chunk violin_plot](assets/fig/violin_plot-1.png)

---
## Overlay data

![plot of chunk violin_plot_data](assets/fig/violin_plot_data-1.png)

---
## Two categorical variables
# Mosaic plot
![plot of chunk mosaic_plot](assets/fig/mosaic_plot-1.png)

----
## Don't end up in a blog for wrong reasons
* https://flowingdata.com/2010/05/14/wait-something-isnt-right-here/
* https://flowingdata.com/2009/11/26/fox-news-makes-the-best-pie-chart-ever/

----
## Conclusions
* Essentially never
	+ Use pie charts (use bar charts instead)
	+ Use dual axes (produce separate plots instead)
	+ Truncate axes
	+ Use 3D unnecessarily
	+ Add color for color's sake (this isn't sales)
* Do
	+ Show the data
	+ Be as clear as possible
	+ Let the data tell the story

----
## Next time
Apply what we've talked about today with R and ggplot!

<div align = "center">
<img src = assets/img/ggplot_cheatsheet.png width = 900 height = 500>
</div>


