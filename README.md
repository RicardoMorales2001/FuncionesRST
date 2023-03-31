---
editor_options: 
  markdown: 
    wrap: 72
output: html_document
---

# FuncionesRST: a demo package

## This is a demo package from R4DS tutorial.

##### Any contact suggestion to the following email "[angel.morales\@est.ikiam.edu.ec](mailto:angel.morales@est.ikiam.edu.ec)"

## Installation and loading

#### Install the latest version from [GitHub] (<https://github.com/RicardoMorales2001/FuncionesRST>) as follow:

# Install

#### if(!require(devtools)) install.packages("devtools")

#### devtools::install_github("<https://github.com/RicardoMorales2001/FuncionesRST.git>")

## Distribution of functions in the package

## *1st function: simple linear regression*

### library(FuncionesCursoR)

Loading required package: ggplot2; dplyr; testthat; tidyverse

### Explanation and description

The reg_linear function is a function in R that performs a linear
regression between two vectors x and y. The main purpose of the function
is to fit a straight line to a two-dimensional (x,y) data set and to
display the straight line fit along with the data on a graph.

The function starts with an if statement to make sure that the vectors x
and y have the same length. If not, the function issues an error message
and stops.

The function then uses the lm function of R to fit a simple linear
regression model of y on x. The lm function takes a formula as an
argument, in which the independent variable (x) is to the right of the
tilde (\~) and the dependent variable (y) is to the left.

After fitting the model, the function uses the plot function to plot the
data, with x-values on the horizontal axis and y-values on the vertical
axis. The abline function is used to add the fitted regression line to
the plot, using the fitted linear regression model as an argument and
setting the color of the line to red.

Finally, the function returns the fitted linear regression model. This
allows the user to inspect the model fit results and obtain information
such as the fitted regression line coefficients, the fitted y values for
any value of x, and model statistics.

## Examples

### 1st example

This example uses simple vectors as data, the next example will use data
from the mtcars library available in RStudio

```{r}
x <- c(95, 85, 72.5, 60, 15, 25, 2, 3, 4, 5)
y <- c(75, 25, 12.5, 18, 20, 26, 2, 4, 5, 6) 
reg_lineal(x, y)
```

```         
Call:
lm(formula = y ~ x)
Coefficients:
(Intercept)            x  
   29.59985     -0.04122 
```

![](images/RGLplot.png){width="543"}

### 2nd example

Example using the mtcars library

```{r}
x <- mtcars$wt
y <- mtcars$mpg
reg_lineal(x, y)
```

```         
Call:
lm(formula = y ~ x)
Coefficients:
(Intercept)            x  
     37.285       -5.344
```

![](images/R2plot.png){width="540"}

## *2nd function: multiple linear regression*

## Lifecycle

FunctionsRST is the first version of a set of functions which were
created with the purpose of being able to automate repetitive processes
when processing data. It is expected over time to implement things in
this package, be it new functions or arguments. The change in the
already existing functions could be given for a better operation or
improving its functionality.

Thank you very much for using this package.
