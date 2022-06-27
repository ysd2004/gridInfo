# R Data: gridInfo

[![DOI](https://zendo.org/badge/504020252.svg)](https://zendo.org/badge/latestdoi/504020252)

This repository is to share the *R* data providing agricultural weights in *acdc* R-package available at R-CRAN. These weights are the number of agricultural cells (NLCD codes 81 and 82) in the PRISM grids, which are converted to the NLCD projection. The State and County FIPS codes are matched with the county's boundary map of 2017 Agricultural Census.

Note: this data is supplementary weights necessary for the R-package *acdc*. The users of *acdc* do NOT need to download this data. For manual calculations, a direct download of this data would be helpful.

GitHub Repository maintained by: Seong Yun\
Department of Agricultural Economics\
Mississippi State University\
**<seong.yun@msstate.edu>**\
**<https://sites.google.com/site/yunsd2004/>**\
*Last updated: June 16, 2022*

------------------------------------------------------------------------

1 Citation
====================================
Please cite this publication;

```r
To cite this data in publications use:

  Yun, Seong D., 2022, "R Data: gridInfo," Data retrieved from the GitHub,
  https://github.com/ysd2004/gridInfo.git.

A BibTeX entry for LaTeX users is

  @misc{,
    title = {R Data: gridInfo},
    author = {Seong D. Yun},
    year = {2022},
    note = {Data retrieved from the GitHub,
    \url{https://github.com/ysd2004/gridInfo.git}}
  }
```

2 Getting started:
==================

All these files are automatically loaded in the use of functions in *acdc* R-package. Generally, users do NOT need to download or load these data files. Downloading these files are only for manual uses. To load *gridInfo2001.rda* in R,

``` r
    ## In R
    load(url("https://raw.github.com/ysd2004/gridInfo/main/gridInfo2001.rda"))
```
For all other years, replace 2001 with one of 2004, 2006, 2008, 2011, 2013, 2016, or 2019 (the most recent NLCD years).

3 Variable Description
==================

*regdata.rda* includes the following variables.
| Column No. | Variable Name  | Description                                          |
|:----:|:------------:|--------------------------------------------------------------|
| 1  | gridNum  | PRISM grid cell number (on NLCD projection)                        | 
| 2  | stco     | State and County FIPS code                                         | 
| 3  | numAg    | Number of agricultural grid cells in a PRISM grid                  | 
| 4  | numAll   | Number of all grid cells in a PRISM grid                           | 
| 5  | portion  | numAg / numAll                                                     |
