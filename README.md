# SignatureAnalysis-CaseStudy

This repository is for reproducing the results of a case study in the ADAGE
signature analysis paper.

The ADAGE signature analysis was performed in R using the
[ADAGEpath](https://github.com/greenelab/ADAGEpath) package.
We also performed the GSEA analysis as a comparison.

Here are the steps to repeat the analysis:

- Clone this repository.
- Install the R packages **readr**, **DT**, **knitr**, **VennDiagram** from CRAN.
```r
install.packages("devtools")
devtools::install_cran(c("readr", "DT", "knitr", "VennDiagram"))
```
- Install **ADAGEpath** from github.
``` r
devtools::install_github("greenelab/ADAGEpath")
```
- Download the GSEA java program from http://software.broadinstitute.org/gsea/downloads.jsp
and put it in the repository folder.
- Knit **case-study.Rmd** in RStudio.