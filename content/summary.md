---
layout: default
title: Take home and extra activities 
nav_order: 9
has_toc: false
---

We went over a lot of material during this workshop! Below is the code that was in the previous section, but all in one code block. Let's go over it to remind ourselves of the different sections of code and how to organize an R script.

``` r
### SET UP THE CODE ####
# install package 
install.packages("tidyverse")

# load package
library(tidyverse)

# set working directory
setwd("C:/Desktop")

# read in the .csv file
kelp_dataset=read.csv("kelp_dataset.csv")

# look at the data
View(kelp_dataset)

# see summary (mean, min, max, and other) of all your variables 
summary(kelp_dataset)

#### FORMAT THE DATA ####
# data looks goods for today. We did not do this but see other workshops!! 

#### DATA ANALYSIS ####
# calculate the mean wet weight of allt he kelps in the kelp_dataset 
mean(kelp_dataset$KelpWetWeight)

# run a corelation test between kelp weight and length 
cor.test(kelp_dataset$KelpWetWeight, kelp_dataset$KelpThallusLength) 

# plot the weigth and length 
plot(kelp_dataset$KelpWetWeight, kelp_dataset$KelpThallusLength)
```

### Extra activities

If you want to practice R some more, come to the Beginner R part 2!

In the mean time, here are some tutorials that go over what we did today and start going over some material we will cover in part 2! These tutorials uses datasets that are built into R, so you do not need to set your working directory or read in files.

I have added a difficulty score next to the links to help you figure out which ones to do next. 1 is most basic, 3 is most advanced.

**Difficulty 1/3**

Beginner R part 2 link (if you can't make the workshop, go over this before going over the other links)

<https://ubc-library-rc.github.io/IntroR/> (previous UBC RC intro to R)

<https://www.statology.org/mtcars-dataset-r/>

<https://www.statology.org/iris-dataset-r/>

**Difficulty 2/3**

<https://rpubs.com/moeransm/intro-iris>

**Difficulty 3/3**

<https://cran.r-project.org/web/packages/explore/vignettes/explore_mtcars.html>

<https://jcoliver.github.io/learn-r/002-intro-stats.html>
