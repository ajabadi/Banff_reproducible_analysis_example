# Reproducible analysis hosted on RStudio Cloud

This repository is an example of how to create a reproducible R project along with a fully reproducible project environemnt using [`renv`](https://rstudio.github.io/renv). It can be cloned onto and tested on [RStudio Cloud](http://rstudio.cloud/). You can run this example analysis report on https://rstudio.cloud/project/1434153.

To adopt this report style using RStudio, follow the following steps:

- Install the `renv` package:
```r
install.packages('renv')
```

- Clone/fork this repository.
- Add your own analysis files to `./notebook`. You might wish to add any other folder structure.
- Add them as child notebooks to `index.Rmd` as shown below (Note that `index.Rmd` is the only file others would render to reproduce the project and should contain all relevant notebooks):
````
```{r, eval=TRUE, child = './path_to_rmd_file.Rmd'}
```
````
- In your RStudio Cloud account, create a project from the GitHub repository and make it public (Project >> Access >> Everyone). Note that the size of the repository for basic accounts is limited to 1GB. It is always possible to pull changes from the source repo from the 'Git' pane.
- Knit/render `index.Rmd` and ensure it fully reproduces the analysis report and the code is also shown (`echo = TRUE` ) where relevant in the report.
