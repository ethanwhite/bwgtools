[![Travis-CI Build Status](https://travis-ci.org/SrivastavaLab/bwg.png?branch=master)](https://travis-ci.org/SrivastavaLab/bwg)

This is an R package for the bromeliad working group rainfall experiment. It uses [rdrop2](https://github.com/karthik/rdrop2) to access you Dropbox account, then uses [readxl](https://github.com/hadley/readxl) to download the data and read it directly into R.  

## Installation

`bwgtools` can be installed directly from Github using devtools:

```r
install.packages("devtools") # if you don't have devtools
library(devtools)
install_github("SrivastavaLab/bwgtools")
```

## First steps

You can read data directly into R . For example:

```r
macae <- read_site_sheet("Macae", "leaf.waterdepths")
```

We can also do some basic checking 

```r
check_names(macae)
```

## Future plans

We want to use this package to store functions which reproduce all of the analyses of the Bromeliad Working Group.

### Licence
We release the code in this repository under the MIT software license. see text of license [here](LICENSE)
