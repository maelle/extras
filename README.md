
<!-- README.md is generated from README.Rmd. Please edit that file -->

# extras

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![R build
status](https://github.com/poissonconsulting/extras/workflows/R-CMD-check/badge.svg)](https://github.com/poissonconsulting/extras/actions)
[![Codecov test
coverage](https://codecov.io/gh/poissonconsulting/extras/branch/master/graph/badge.svg)](https://codecov.io/gh/poissonconsulting/extras?branch=master)
[![License:
MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![CRAN
status](https://www.r-pkg.org/badges/version/extras)](https://cran.r-project.org/package=extras)
<!-- ![CRAN downloads](https://cranlogs.r-pkg.org/badges/extras) -->

<!-- badges: end -->

`extras` provides basic functions for Bayesian analyses; functions to
summarise MCMC samples; and R translations of a handful of common
functions from modeling languages such as BUGS/JAGS and C++ (STAN and
TMB).

## Installation

<!-- To install the latest release from [CRAN](https://cran.r-project.org) -->

To install the developmental version from
[GitHub](https://github.com/poissonconsulting/extras)

``` r
# install.packages("remotes")
remotes::install_github("poissonconsulting/extras")
```

## Demonstration

### Summarise MCMC Samples

The `extras` package provides functions to summarise MCMC samples like
`svalue()` which gives the *surprisal value* (Greenland, 2019)

``` r
library(extras)
set.seed(1)
x <- rnorm(100)
svalue(rnorm(100))
#> [1] 0.3183615
svalue(rnorm(100, mean = 1))
#> [1] 1.704015
svalue(rnorm(100, mean = 2))
#> [1] 3.850857
svalue(rnorm(100, mean = 3))
#> [1] 5.073249
```

## R translations

The package also provides R translations of BUGS/JAGS functions such as
`log<-` and `logit<-`.

``` r
mu <- NULL
log(mu) <- 1
mu
#> [1] 2.718282
```

And STAN (C++) functions such as `pow()`.

``` r
2^3 # base R
#> [1] 8
pow(2, 3)
#> [1] 8
```

## References

Greenland, S. 2019. Valid P -Values Behave Exactly as They Should: Some
Misleading Criticisms of P -Values and Their Resolution With S -Values.
The American Statistician 73(sup1): 106–114.
<http://doi.org/10.1080/00031305.2018.1529625>.

## Contribution

Please report any
[issues](https://github.com/poissonconsulting/extras/issues).

[Pull requests](https://github.com/poissonconsulting/extras/pulls) are
always welcome.

## Code of Conduct

Please note that the extras project is released with a [Contributor Code
of
Conduct](https://contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html).
By contributing to this project, you agree to abide by its terms.
