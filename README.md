
<!-- README.md is generated from README.Rmd. Please edit that file -->

# nameformeR

<!-- badges: start -->

[![R-CMD-check](https://github.com/UBC-MDS/nameformeR/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/UBC-MDS/nameformeR/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

nameformeR is an R translation of our python package
[nameforme](https://github.com/UBC-MDS/nameforme)

A helper package that can be used to generate names based on the
dateset. This could be used to come up with baby names, character names,
pseudonyms, etc.

Source Data: Contains baby names born in the United States for each year
from 1880 to 2017, and the number of children of each sex given each
name. Names must appear at least 5 times in the each year to be
included. (Source: <http://www.ssa.gov/oact/babynames/limits.html>)

This package is similar to an existing R package called
[randomNames](https://cran.r-project.org/web/packages/randomNames/) in
CRAN. This package focuses on generating random first and last names by
ethnicity, whereas ours only generates first names, but provides more
helper methods for users to customize what type of names to generate,
including the ability to generate similar sounding names.

## Functions Included

Note that the name of functions are not finalized. They are subject to
change.

The package is an assimilation of four independent functions:

- `find_name`: Generate a random set of 10 suggested baby names based on
  the given limitations.

- `find_unisex_name`: Generate the a random set of suggested neutral
  baby names based on the given limitation and baby names in the past
  years.

- `find_old_name`: Generate a random set of suggested neutral(by
  default) baby names based on the given time period and sex.

- `find_similar_name`: Generate a random list of names that sound
  similar to a given user input name.

## Dependencies

- comparator (\>= 0.1.2),
- stringr (\>= 1.5.0),
- dplyr (\>= 1.0.10),
- readr (\>= 2.1.3)

## License

`nameforme` was created by Daniel Cairns, Eyre Hong, Bruce Wu, Zilong Yi
(UBC MDS). It is licensed under the terms of the MIT license.
