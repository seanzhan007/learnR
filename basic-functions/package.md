

# Package functions

In R, packages play an indispensable role in data analysis and visualization. In fact, R is only a tiny core and is built on several basic packages. A package is nothing special but a box of predefined functions which are often designed to be general enough to solve a wide range of similar problems.

A package to R is a bit like a theory to mathematics or a toolbox to statistics. With a well-designed package, we don't have to invent the same wheel again and again, which allows us to focus more on the problem we are trying to solve.

R is powerful not only because of its rich source of packages but also because of the well-maintained package archive system called The Comprehensive R Archive Network, or [CRAN](http://cran.r-project.org/). The source code of R and thousands of packages are archived in this system. We can even look at the [table](http://cran.r-project.org/web/packages/available_packages_by_date.html) that shows all the packages currently available.

To download and install a package in R is extremely easy. Just call

```r
install.packages("ggplot2")
```

and R will automatically download the package, install, and sometimes compiles the package.

Nowadays, many package authors choose a website called [GitHub](http://github.com/) to host their work because it's very easy for version control and community development, thanks to the well-designed issue tracking systems. Some authors even do not release their work to CRAN, and others only release the stable versions to CRAN and keep new versions with brand new features on GitHub.

To keep a package up to date with the latest development version which often has new features or has fixed some bugs, we can directly install the package via `devtools` package.

```r
install.packages("devtools")
devtools::install_github("hadley/ggplot2")
```

`devtools` will download the source code from GitHub and makes it a package for you.
