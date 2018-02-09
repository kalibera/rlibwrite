---
title: "Running WhiteStripe on T1- and T2-weighted Imaging"
author: "John Muschelli"
date: "2018-02-09"
output: rmarkdown::html_vignette
vignette: >
  %\VignetteIndexEntry{Running WhiteStripe on T1- and T2-weighted Imaging}
  %\VignetteEngine{knitr::rmarkdown}
  %\VignetteEncoding{UTF-8}
---

# Downloading the data

First, we would like to make sure we have some data to work with.  The data is not located directly in the installed package to make it lightweight and some other repository restrictions. 

To download the test data, we will use the WhiteStripe function `download_img_data`:


```r
library(WhiteStripe)
download_img_data()
```

```
## Warning in download.file(url, urlfile, quiet = TRUE): URL http://
## muschellij2.github.io/WhiteStripe/T1Strip.nii.gz: cannot open destfile '/
## var/scratchro/tomas/QA/R-74238/lib/WhiteStripe/T1Strip.nii.gz', reason
## 'Read-only file system'
```

```
## Warning in download.file(url, urlfile, quiet = TRUE): download had nonzero
## exit status
```

```
## Warning in download.file(url, urlfile, quiet = TRUE): URL http://
## muschellij2.github.io/WhiteStripe/T2Strip.nii.gz: cannot open destfile '/
## var/scratchro/tomas/QA/R-74238/lib/WhiteStripe/T2Strip.nii.gz', reason
## 'Read-only file system'
```

```
## Warning in download.file(url, urlfile, quiet = TRUE): download had nonzero
## exit status
```

```
## [1] FALSE
```
## Getting the filenames

Once the data is downloaded, we can access the files using the `ws_img_data` function:


```r
files = ws_img_data()
```

```
## Warning in ws_img_data(): Files are not downloaded, use download_img_data
## first!
```

# Reading in the data

We will focus on the T1-weighted image here:
















