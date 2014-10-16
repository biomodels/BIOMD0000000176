# BIOMD0000000176: Conant2007_WGD_glycolysis_2A3AB

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000176.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000176.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000176 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This a model from the article:  
**Increased glycolytic flux as an outcome of whole-genome duplication in yeast.**   
Conant GC, Wolfe KH _Mol. Syst. Biol._ [2007 ; Volume: 3 (Issue: )]: 129
[17667951](http://www.ncbi.nlm.nih.gov/pubmed/17667951) ,  
**Abstract:**   
After whole-genome duplication (WGD), deletions return most loci to single
copy. However, duplicate loci may survive through selection for increased
dosage. Here, we show how the WGD increased copy number of some glycolytic
genes could have conferred an almost immediate selective advantage to an
ancestor of Saccharomyces cerevisiae, providing a rationale for the success of
the WGD. We propose that the loss of other redundant genes throughout the
genome resulted in incremental dosage increases for the surviving duplicated
glycolytic genes. This increase gave post-WGD yeasts a growth advantage
through rapid glucose fermentation; one of this lineage's many adaptations to
glucose-rich environments. Our hypothesis is supported by data from enzyme
kinetics and comparative genomics. Because changes in gene dosage follow
directly from post-WGD deletions, dosage selection can confer an almost
instantaneous benefit after WGD, unlike neofunctionalization or
subfunctionalization, which require specific mutations. We also show
theoretically that increased fermentative capacity is of greatest advantage
when glucose resources are both large and dense, an observation potentially
related to the appearance of angiosperms around the time of WGD.

  
  

The original model submitted by the authors was slightly altered and now
comprises the models originally submitted as MODEL2426780967, MODEL2427021978,
MODEL2427095802. It reproduces figures 2A,3A and 3B from the publication.

This model uses the glycolysis model from Pritchard and Kell (2002) with an
additional parameter, **WGD_E** , to adjust for the differing enzyme
conzentrations before the whole genome duplication (WGD) and parameters
**fV_xxx** that adjust the **Vmax** of the different reactions (xxx eg. HXT or
PYK).  
Figure 3A from the article can be reproduced by changing the value of the
parameters **fV_xxx** to 0.9 indiviually, with xxx signifying the different
enzymes (HXT, HXK ...)  
Figure 3B from the publication can be reproduced by setting the parameter
**WGD_E** to 0.75 and individually setting the parameters **fV_xxx** to 1.333.  
To reproduce figure 2A from the article change the parameter **WGD_E** in the
range between 0.65 and 1.0.

This model originates from BioModels Database: A Database of Annotated
Published Models (http://www.ebi.ac.uk/biomodels/). It is copyright (c)
2005-2012 The BioModels.net Team.  
For more information see the [terms of
use](http://www.ebi.ac.uk/biomodels/legal.html) .  
To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


