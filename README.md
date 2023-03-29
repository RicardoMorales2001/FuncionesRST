FuncionesRS: a demo package
===============================================

## This is a demo package from R4DS tutorial.
##### Any contact suggestion to the following email "angel.morales@est.ikiam.edu.ec"

## Installation and loading

#### Install the latest version from [GitHub] (https://github.com/RicardoMorales2001/FuncionesRST) as follow:


# Install
#### if(!require(devtools)) install.packages("devtools")
#### devtools::install_github("https://github.com/RicardoMorales2001/FuncionesRST.git")


Distribution of functions in the package
------------
## 1st function

 r
### library(FuncionesCursoR)
#### Loading required package: ggplot2; dplyr; testthat; tidyverse
### Create some data format
# :::::::::::::::::::::::::::::::::::::::::::::::::::
set.seed(1234)
x <- c(95, 85, 72.5, 60, 15, 25, 2, 3, 4, 5)
y <- c(75, 25, 12.5, 18, 20, 26, 2, 4, 5, 6)
reg_lineal(x, y)


