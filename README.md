PheNorm
================

## Overview

This package provides an unsupervised phenotyping algorithm, PheNorm,
for electronic health record (EHR) data. A human-annotated training set
with gold-standard disease status labels is usually required to build an
algorithm for phenotyping based on a set of predictive features.
PheNorm, however, does not require expert-labeled samples for training.

The algorithm combines the most predictive variables, such as the count
of the main International Classification of Diseases (ICD) codes, with
other EHR features. Those include for example health utilization and
processed clinical note data. PheNorm aims to obtain a score for
accurate risk prediction and disease classification. In particular, it
normalizes the surrogate to resemble gaussian mixture and leverages the
remaining features through random corruption denoising. PheNorm
automatically generates phenotyping algorithms and demonstrates the
capacity for EHR-driven annotations to scale to the next level -
phenotypic big data.

The data consists of ICD codes and additional features.

The output consists of, on one hand, for each individual, the predicted
probability of the risk of having the phenotype; on the other hand, the
coefficient beta corresponding to all the features additional to the ICD
codes.

The main steps of the algorithm are presented in the following flowchart
:
<https://pubmed.ncbi.nlm.nih.gov/29126253/#&gid=article-figures&pid=figure-1-uid-0>.

Next, we propose a simple example in which we fit PheNorm to a simulated
dataset.

## Installation

Load the package into R.

``` r
#library(PheNorm)
```

## Example on simulated dataset

``` r
#set.seed(1234)
#dat <- read.csv()
```

Apply the PheNorm
algorithm

``` r
#fit.phenorm=PheNorm.Prob("ICD", "utl", fit.dat, nm.X = NULL, corrupt.rate=0.3,
#                         train.size=nrow(fit.dat))
```
