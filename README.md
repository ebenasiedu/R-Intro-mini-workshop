# R-Intro-mini-workshop (August 19 - 20, 2023)
Hello! Welcome to this introductory R mini-workshop. 

---------------------------------------------------------
## Installing R, R studio, and Packages
Please follow the instructions below to install R, R studio, and some packages on your computer prior to the workshop
This will save us lots of time! 
Thank you

Please follow these guidelines to install R and some packages on your machine.

This will save us time during the workshop :)

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
packages <- c("tidyverse", "tidymodels", "tibble", "ggrepel","corrplot", "readxl", "ggpubr", 
              "viridis", "ggsci", "reshape2", "pheatmap", "patchwork", "emmeans",  "mlbench")
new_packages <- packages[!(packages %in% installed.packages()[,"Package"])]
if(length(new_packages)) install.packages(new_packages)

all_packages <- c("tidyverse", "tidymodels", "tibble", "ggrepel","corrplot", "readxl", "ggpubr", 
              "viridis", "ggsci", "reshape2", "pheatmap", "patchwork", "emmeans", "mlbench")

if(sum(!(all_packages %in% installed.packages()[, "Package"]))) {
  stop("Not all required packages are installed!")
} else {
  message("Everything is set up correctly. You are ready for the workshop!")
}
```


---------------------------------------------------------
## Zoom Link
We'll have two sessions per day (afternoon and evening sessions), 2-3 hrs per session.

---------------------------------------------------------
**Afternoon session: 8am - 10:30am (EST) or 12pm - 2:30pm (GMT)**

**Evening session: 12:30pm - 3pm (EST) or 4:30pm - 7pm (GMT)**

---------------------------------------------------------
Please use this link to join the fun!

https://unm.zoom.us/j/2116510521

Passcode: Dabs

---------------------------------------------------------
