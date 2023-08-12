# R-Intro-mini-workshop

## Installing R, R studio, and Packages

Please follow these guidelines to install R and some packages on your machine.

This will save us time during the workshop :)

`Windows` `Mac` `Linux`

1.  Download and install R from here: <https://cran.rstudio.com/>

2.  Download RStudio here: <https://posit.co/download/rstudio-desktop/>


## Install some packages

Please copy, paste, and run the code below in your installed R studio.

We'll briefly walk through what each line mean during the workshop :) 

``` r
packages <- c("tidyverse", "corrplot", "readxl", "tibble", "ggpubr", 
              "viridis", "ggsci", "reshape2", "pheatmap", "ComplexHeatmap", 
              "patchwork", "emmeans","caret")
new_packages <- packages[!(packages %in% installed.packages()[,"Package"])]
if(length(new_packages)) install.packages(new_packages)

all_packages <- c("tidyverse", "corrplot", "readxl", "tibble", "ggpubr", 
              "viridis", "ggsci", "reshape2", "pheatmap", "ComplexHeatmap", 
              "patchwork", "emmeans","caret")

if(sum(!(all_packages %in% installed.packages()[, "Package"]))) {
  stop("Not all required packages are installed!")
} else {
  message("Everything is set up correctly. You are ready for the workshop!")
}
```
