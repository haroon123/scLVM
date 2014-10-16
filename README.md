#scLVM


##What is scLVM?

scLVM is a modelling framework for single-cell RNA-seq data that can be used to dissect the observed heterogeneity into different sources, thereby allowing for the correction of confounding sources of variation. 

By Florian Buettner, Paolo Casale and Oliver Stegle

##Philosophy

Observed heterogeneity in single-cell profiling data is multi-factorial. scLVM provides an efficient framework for unravelling this heterogeneity, correcting for confounding facotrs and facilitating unbiased downstream analyses. scLVM builds on Gaussian process latent variable models and mixed linear models. Our modelling approach is based on efficient inference algorithms implemented in [LIMIX](https://github.com/PMBio/limix).

##Installation:

* scLVM is particularly easy to install using the [anaconda](https://store.continuum.io/cshop/anaconda) python distribution.
 
* It requires Python 2.7 with
  - scipy, h5py, numpy, pylab

* scLVM relies heavily on [limix](https://github.com/PMBio/limix), which can be installed using ``pip install limix`` on most systems.

* If you would like to use the non-linear GPLVM for visualisation, you require the [GPy](https://github.com/SheffieldML/GPy) package. This can be installed using `pip install GPy` 

* Preprocessing steps are executed in R and require R>3.0:
For an example of how raw counts can be processed appropriately, see R/transform_counts_Tcells.R. A more extensively commented markdown version of the script can be found here: transform_counts_demo.Rmd.

##How to use scLVM?

A good starting point are the [tutorials](https://github.com/PMBio/scLVM/blob/master/tutorials).

For a example that shows how scLVM can be applied to the T-cell data considered in Buettner et al. [2], we have prepared a notebook that can be viewed [interactively](http://nbviewer.ipython.org/github/pmbio/scLVM/blob/master/tutorials/tcell_demo.ipynb) or alternatively as [PDF](https://github.com/PMBio/scLVM/blob/master/tutorials/tcell_demo.pdf) export.


 ##Problems ?

If you want to use scLVM and encounter any issues, please contact us by email: scLVM-dev@ebi.ac.uk

##License
See [LICENSE] https://github.com/PMBio/scLVM/blob/master/license.txt

###References
Buettner F, Natarajan KN, Casale FP, Proserpio V, Scialdone A, Theis FJ, Teichmann SA, Marioni JC & Stegle O, 2014. Accounting for cell-to-cell heterogeneity in single-cell RNA-Seq data reveals novel structure between cells, Nat Biotech, in press.
