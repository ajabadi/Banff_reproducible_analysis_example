# Reproducible analysis hosted on RStudio Cloud

This repository is an example on how to create a reproducible analysis which uses a fully reproducible project environemnt using [`renv`](https://rstudio.github.io/renv) and can be indepently tested on RStudio Cloud.


If you would like to adopt this report style using RStudio:

- Install `renv` package
```r
install.packages('renv')
```

- Clone/fork this repository
- Add your own analysis files to `./notebook`
- Add them as child notebooks to `index.Rmd` as shown
- on your RStudio Cloud account, create a public project from the repository
- Knit/render `index.Rmd` and ensure it fully reproduces the analysis report and the code is also shown (`echo = TRUE` ) where relevant in the report
