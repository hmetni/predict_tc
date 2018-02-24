# Predict the Critical Temperature of a Superconductor

The first thing you need to do is to make sure you have installed R.  Go to https://cloud.r-project.org/ to install the latest version of R.

You need two R packages.  Open up the R gui and run the following command.  If a pop up window opens up with title "Secure CRAN mirror", just pick "0-Cloud [https]" and hit OK.  
```r
install.packages(c("ranger","CHNOSZ"))
```
You only need to run the above command once; you'll never to install these packages unless you download a new R version.

Now you need to make these packages available to your current R session.  You need to do this EVERY time you want to use these packages:
```r
library(ranger)
library(CHNOSZ)
```

Next, download the file auxiliary.RData.  Make sure you know where in your computer you downloaded this file.  This file contains all the data and auxiliary functions to create the prediction model.

Please read this next line carefully: **MAKE SURE YOUR R SESSION'S WORKING DIRECTORY IS SET TO WHERE YOU DOWNLOADED THIS FILE**.  

You can do this in two ways: (1) Go to R Console, then go to menu path File, and then to "Change dir...", or (2) use ```setwd ``` command.  (I do not use RStudio.)

Run:
```r
load("auxiliary.RData")
```
