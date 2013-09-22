locfdr-python v0.1
==================

Python variant of Efron, Turnbull, and Narasimhan's R function locfdr() v1.1-7, which computes local false discovery rates. See http://cran.r-project.org/web/packages/locfdr/ for more information.

This port is very literal interpretation of the augmented version of locfdr at https://github.com/alyssafrazee/derfinder/blob/master/R/locfdrFit.R : the organization of the code parallels the original where efficient, and variable and function names are the same as in R. Rfunctions.py contains Python functions designed to mimic R's idiosyncratic implementations of interpolation.

Requirements: Python 2.7.x, scipy, numpy, matplotlib, pandas, and statsmodels. The code was tested on Anaconda, which contains Python 2.7.5, scipy 0.12.0, numpy 1.7.1, pandas 0.12.0, statsmodels 0.5.0, and matplotlib 1.3.0. This distribution is available at https://store.continuum.io/cshop/anaconda/.

Installation: (will use distutils)

Usage:

from locfdr import locfdr

\# Initialize data here, as described in http://cran.r-project.org/web/packages/locfdr/locfdr.pdf .

results = locfdr(zz)