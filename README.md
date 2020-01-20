
<!-- README.md is generated from README.Rmd. Please edit that file -->

# extras

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Travis build
status](https://travis-ci.com/poissonconsulting/extras.svg?branch=master)](https://travis-ci.com/poissonconsulting/extras)
[![AppVeyor build
status](https://ci.appveyor.com/api/projects/status/github/poissonconsulting/extras?branch=master&svg=true)](https://ci.appveyor.com/project/poissonconsulting/extras)
[![Codecov test
coverage](https://codecov.io/gh/poissonconsulting/extras/branch/master/graph/badge.svg)](https://codecov.io/gh/poissonconsulting/extras?branch=master)
[![License:
MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
<!-- [![Tinyverse status](https://tinyverse.netlify.com/badge/extras)](https://CRAN.R-project.org/package=extras) -->
<!-- [![CRAN status](https://www.r-pkg.org/badges/version/extras)](https://cran.r-project.org/package=extras) -->
<!-- ![CRAN downloads](https://cranlogs.r-pkg.org/badges/extras) -->
<!-- badges: end -->

extras provides a template for a new R package.

It includes useful internal functions.

## Installation

<!-- To install the latest release from [CRAN](https://cran.r-project.org) -->

To install the developmental version from
[GitHub](https://github.com/poissonconsulting/extras)

``` r
# install.packages("remotes")
remotes::install_github("poissonconsulting/extras")
```

To install the latest developmental release from the Poisson drat
[repository](https://github.com/poissonconsulting/drat)

``` r
# install.packages("drat")
drat::addRepo("poissonconsulting")
install.packages("extras")
```

## Demonstration

In order to create a new package the user should go to the extras
[GitHub repository](https://github.com/poissonconsulting/extras) and
choose ‘Use this template’.

extras includes files used for development of Shiny applications. To
remove these from the repository, run:

``` r
extras:::cannibalise_shiny(getwd())
```

## Information

For more information see the [Get
Started](https://poissonconsulting.github.io/extras/articles/extras.html)
vignette.

## Contribution

Please report any
[issues](https://github.com/poissonconsulting/extras/issues).

[Pull requests](https://github.com/poissonconsulting/extras/pulls) are
always welcome.

Please note that this project is released with a [Contributor Code of
Conduct](https://github.com/poissonconsulting/extras/blob/master/CODE_OF_CONDUCT.md).
By contributing, you agree to abide by its terms.
