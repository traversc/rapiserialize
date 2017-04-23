## RApiSerialize [![Build Status](https://travis-ci.org/eddelbuettel/rapiserialize.svg)](https://travis-ci.org/eddelbuettel/rapiserialize) [![License](http://img.shields.io/badge/license-GPL%20%28%3E=%202%29-brightgreen.svg?style=flat)](http://www.gnu.org/licenses/gpl-2.0.html) [![CRAN](http://www.r-pkg.org/badges/version/RApiSerialize)](http://cran.rstudio.com/package=RApiSerialize) [![Downloads](http://cranlogs.r-pkg.org/badges/RApiSerialize?color=brightgreen)](http://www.r-pkg.org/pkg/RApiSerialize)

This package provides C-level serialization as R does for itself. It is
useful if you are writing C (or C++) code in an R package which needs to
(un)serialize R data structures, and wants to do it faster than calling the
corresponding R level function would do.

In other words, this is somewhat specialised for situation of high data
throughput, or other cases of a need for high performance.  Or maybe you are
just impatient and want the result faster.

This package owes a lot of debt to the
[Rhpc](http://cran.rstudio.com/package=Rhpc) package by 
Ei-ji Nakama and Junji Nakano. It gave me the idea of using a copy of the
code which is not exported by R itself.  And of course credit is due to the R
Core team for writing R, and the code used here.

### Example use

See my [RcppRedis](https://github.com/eddelbuettel/rcppredis) package for use
of this package

### Copyrights

Copyrights are held by the respective authors, in particular
Ei-ji Nakama and Junji Nakano as well as the R Core Team
for the intial version of the actual serialization code, and
Dirk Eddelbuettel for subsequent modificatons and the remainder
of the package.

### License

GPL (>= 2)

