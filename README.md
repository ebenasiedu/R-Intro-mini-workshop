# R-Intro-mini-workshop (August 26 - 27, 2023)

Access videos here: https://drive.google.com/drive/folders/1U3OeEH1yAkct97Jc0aRGJKxBqAzvK5jp?usp=sharing

---------------------------------------------------------
## Installing R, R studio, and Packages
Please follow the instructions below to install R, R studio, and some packages on your computer prior to the workshop.

This will save us time during the workshop :)

Thank you

1.  Download and install R from here: <https://cran.rstudio.com/>

2.  Download RStudio here: <https://posit.co/download/rstudio-desktop/>

Watch these videos for additional guidance:

`Windows:` https://www.youtube.com/watch?v=YrEe2TLr3MI

 `Mac:` https://www.youtube.com/watch?v=JqV-USGR6AA
 
 `Linux:` https://www.youtube.com/watch?v=HEDhbgOEm8o

---------------------------------------------------------
## Install some packages

Please copy, paste, and run the code below in your installed R studio.

We'll briefly walk through what each line mean during the workshop :) 

``` r
packages <- c("tidyverse", "tidymodels", "tibble", "ggrepel","corrplot", "readxl", "ggpubr", "stringr", "dslabs",
              "ggcorrplot","viridis", "ggsci", "reshape2", "pheatmap", "patchwork", "emmeans",  "mlbench")
new_packages <- packages[!(packages %in% installed.packages()[,"Package"])]
if(length(new_packages)) install.packages(new_packages)

all_packages <- c("tidyverse", "tidymodels", "tibble", "ggrepel","corrplot", "readxl", "ggpubr",  "stringr", "dslabs",
              "ggcorrplot", "viridis", "ggsci", "reshape2", "pheatmap", "patchwork", "emmeans", "mlbench")

if(sum(!(all_packages %in% installed.packages()[, "Package"]))) {
  stop("Not all required packages are installed!")
} else {
  message("Everything is set up correctly. You are ready for the workshop!")
}
```


---------------------------------------------------------
