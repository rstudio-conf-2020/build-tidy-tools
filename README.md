
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Building Tidy Tools

### rstudio::conf 2020

by Charlotte Wickham and Hadley Wickham

-----

:spiral\_calendar: January 27 and 28, 2020  
:alarm\_clock: 09:00 - 17:00  
:hotel: Plaza A (Lobby Level)  
:writing\_hand: [rstd.io/conf](http://rstd.io/conf)

-----

## Overview

This is a two-day hands on workshop for those who have embraced the
tidyverse and now want to expand it to meet their own needs. We’ll
discuss API design, functional programming tools, the basics of object
design in S3, and the tidy eval system for NSE.

  - Learn efficient workflows for developing high-quality R functions,
    using the set of conventions codified by a package. You’ll also
    learn workflows for unit testing, which helps ensure that your
    functions do exactly what you think they do.
  - Master the art of writing functions that do one thing well and can
    be fluently combined together to solve more complex problems. We’ll
    cover common function writing pitfalls and how to avoid them.
  - Learn how to write collections of functions that work well together,
    and adhere to existing conventions so they’re easy to pick up for
    newcomers.

You should take this workshop if you have experience programming in R
and want to learn how to tackle larger scale problems. You’ll get the
most from it if you’re already familiar with functions and are
comfortable with R’s basic data structures (vectors, matrices, arrays,
lists, and data frames). Note: There is ~30% overlap in the material
with Hadley Wickham’s previous “R Masterclass”. However, the material
has been substantially reorganised, so if you’ve taken the R Masterclass
in the past, you’ll still learn a lot in this class.

## Learning objectives

## Materials

Materials will be made available on
[github](https://github.com/rstudio-conf-2020/build-tidy-tools). If you
are using an organization-issued laptop, you may want to verify before
you arrive that you can access GitHub.

The materials will evolve as the workshop approaches, so if you want to
pre-download the materials, please wait until the day before the
workshop.

## Setup

<!-- Fix later to generate from content of repo like https://github.com/hadley/tidy-tools/blob/master/README.Rmd -->

Please make sure you’ve installed the following packages:

``` r
install.packages("devtools")
install.packages(c("fs", "glue", "lobstr", "rematch2", "sloop", "vctrs"))
devtools::install_github("r-lib/itdepends")
```

``` r
# You may also need:
install.packages(c("ggplot2", "dplyr", "stringr"))

# And get the package we'll work with later:
usethis::create_from_github("hadley/fordogs", fork = FALSE)

# if you see an error about "unsupported protocol", try this:
usethis::create_from_github("hadley/fordogs", fork = FALSE, protocol = "https")
```

<!-- 
* When you're done, put a green post-it on your computer. 
* If you need help, put up a pink post-it.
-->
