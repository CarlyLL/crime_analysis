## Crime analysis in R

This growing repository contains scripts that enable users to load, tidy, manipulate, summarise and (interactively) visualise police recorded crime data in R.

#### Getting started

Download R from [https://cran.r-project.org](https://cran.r-project.org). 

Then load some sample crime data into your R session:

```
download.file("https://raw.github.com/cat-lord/crime_analysis/master/data/crime_data.csv", 
              destfile = "~/crime_data.csv", method = "curl") 

setwd("~/")

crimes <- read.csv("crime_data.csv", header = T)
```

The data are crimes recorded by Greater Manchester Police between December 2014 and November 2015 which were downloaded from [data.police.uk](https://data.police.uk).

The scripts and [shiny](http://shiny.rstudio.com) apps will work with any data downloaded from [data.police.uk](https://data.police.uk) but they will need to share the same structure, i.e. be [tidy](https://vimeo.com/33727555) first. Follow the [tidying_data](https://github.com/cat-lord/crime_analysis/blob/master/data/tidying_data.R) script for instructions.

#### The scripts
  
* [summary statistics](https://github.com/cat-lord/crime_analysis/blob/master/scripts/summary_statistics.R)
* [the 80-20 rule](https://github.com/cat-lord/crime_analysis/blob/master/scripts/the_80-20_rule.R)
* [repeat locations](https://github.com/cat-lord/crime_analysis/blob/master/scripts/repeat_locations.R)
* calculating rates of crime (forthcoming)
* point pattern analysis (forthcoming)

#### Data visualisations

There are several scripts to create simple [data visualisations](https://github.com/cat-lord/crime_analysis/tree/master/data_visualisations) including Cleveland-style dotplots and calendar heatmaps.

#### Shiny apps

This repository includes several simple [shiny apps](https://github.com/cat-lord/crime_analysis/tree/master/shinyapps) that allow users to interactively visualise crime data.

* [bar charts](https://github.com/cat-lord/crime_analysis/tree/master/shinyapps/bar_charts)
* [dotplot](https://github.com/cat-lord/crime_analysis/tree/master/shinyapps/dotplot)
* [time series](https://github.com/cat-lord/crime_analysis/tree/master/shinyapps/time_series)

#### Links

* Clarke, R.V., & J.E. Eck. (2003). [Become a Problem Solving Crime Analyst In 55 small steps](http://www.popcenter.org/library/reading/pdfs/55stepsUK.pdf). Jill Dando Institute of Crime Science, University College London.
* Tompson, L., Johnson, S., Ashby, M., Perkins, C., & Edwards, P. (2015). [UK open source crime data: accuracy and possibilities for research](http://www.tandfonline.com/doi/full/10.1080/15230406.2014.972456). Cartography and Geographic Information Science, 42(2), 97-111.

