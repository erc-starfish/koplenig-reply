# koplenig-reply

This repository contains data and data analysis code for the following paper:

> Kauhanen, H., Einhaus, S. & Walkden, G. (2022) Language structure is influenced by the proportion of non-native speakers: A reply to Koplenig (2019).


## Data

The data resides in the `data/` directory as a comma-separated values file. See the `README.md` file in that directory for further details.


## Analysis

To run the data analysis, navigate to the `R/` directory and, from an R session, call:

```r
rmarkdown::render("analysis.Rmd", output_file="../analysis.pdf")
```

The report will be outputted in `analysis.pdf`; additionally, plots are saved in the `plots/` folder.

R packages `ggplot2`, `gridExtra` and `rmarkdown` are required. Tested using R version 4.0.4.


## Acknowledgements

This research was funded by the European Research Council as part of project STARFISH (851423). We are also grateful to the Department of Linguistics of the University of Konstanz for making Ethnologue available to us.
