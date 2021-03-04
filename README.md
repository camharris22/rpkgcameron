
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rpkgcameron

<!-- badges: start -->

<!-- badges: end -->

The goal of rpkgcameron is to make working with factors easier (and to
get completion marks for my assignment\!)

## Installation

You can install the released version of rpkgcameron from
[CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("rpkgcameron")
```

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("camharris22/rpkgcameron")
```

## Demonstration

This is a basic example which shows you how to concatenate two factors:

``` r
library(rpkgcameron)
a <- factor(c("character", "hits", "your", "eyeballs"))
b <- factor(c("but", "integer", "where it", "counts"))
```

As we can see, concatenate doesn’t work properly here:

``` r
c(a, b)
#> [1] 1 3 4 2 1 3 4 2
```

The function `fbind()` to the rescue\!

    #> [1] character hits      your      eyeballs  but       integer   where it 
    #> [8] counts   
    #> Levels: but character counts eyeballs hits integer where it your
