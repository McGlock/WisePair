###**WisePair**
* * *
####What is it used for?
wisepair is a set of python scripts built to address two issues in individual-based
genetic tracking studies.  
1) Sampling scheme design to maximize resampling a set number of individuals.  
2) Confidently identifying individuals who have been resampled in a data-set.  
* * *
####There are 3 main scripts in the core of WisePair:  
**_beanbag.py_**  
The beanbag.py script was specifically designed to build virtual individual genotypes of a population to be used in simulated sampling.  This design was based on user-supplied criteria such as number of individuals in the population, number of loci, and allelic frequencies.  In addition, this script incorporated genotyping error rates during sampling.  
**_wisepair.py_**  
The second script, wisepair.py, was created to determine the number of re-samples within a specified data set (real or virtual) through allelic pairwise comparisons.  wisepair.py determined the number of re-samples within a virtual data set, determined the number of re-samples within an actual data using specified threshold simulations, estimated the number of errors for re-samples, and determined whether re-samples can be distinguished from non-re-samples.  
**_optimagic.py_**  
The final script, optimagic.py, utilized outputs from both beanbag.py and wisepair.py to develop optimal sampling designs for individual based studies.  beanbag.py and wisepair.py were used to produce a threshold “score” with which we could compare samples to the field data set and subsequent simulations in OPTIMAGIC.py  
* * *

