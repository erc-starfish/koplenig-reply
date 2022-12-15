# koplenig-reply

This repository contains data and data analysis code for the following paper:

> Kauhanen, H., Einhaus, S. & Walkden, G. (2022) Language structure is influenced by the proportion of non-native speakers: A reply to Koplenig (2019).


## Data

The data resides in the `data/` directory as comma-separated values files. See the `README.md` file in that directory for further details.


## Analysis

To run the data analysis, navigate to the `R/` directory and, from an R session, call:

```r
rmarkdown::render("analysis.Rmd", output_file="../analysis.pdf")
```

The report will be outputted in `analysis.pdf`; additionally, plots are saved in the `plots/` folder.

This takes about a minute on a modern computer (tested using R version 4.0.4).

A number of R packages are needed; to install them, type:

```{r}
install.packages(c("lme4", "lmerTest", "mice", "broom.mixed", "lattice", "effects", "gridExtra"))
```


## Acknowledgements

The work reported here was funded by the European Research Council as part of project STARFISH (851423). Access to Ethnologue was funded by the Communication, Information, Media Centre (KIM) of the University of Konstanz.
