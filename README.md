
![](assets/SCOT_logo.png)

# Single-Cell alignment using Optimal Transport (SCOT)

SCOT is a python tool for performing unsupervised alignment of single-cell multi-omics datasets. Its methodology is detailed in the pre-print "[Gromov-Wasserstein based optimal transport for aligning single-cell multi-omics data](https://www.biorxiv.org/content/10.1101/2020.04.28.066787v2)" (bioRxiv link: https://www.biorxiv.org/content/10.1101/2020.04.28.066787v2)

**Note:** We are currently in the process of updating our repository for better documentation, code readibility, and complete set of experiments. You will be able to check out the demonstrations and documentations here: https://rsinghlab.github.io/SCOT/, as well as on our Jupyter Notebooks in the repository.  

### SCOT v.0.2.0  
Changes from the previous version:  
**1)** Extensions to cases with differing representation of cell types between domains with unbalanced OT   
We are thankful for [Stephen Zhang](http://zsteve.phatcode.net/about/)'s [contributions](https://github.com/zsteve/SCOT) to our repository with the integration of [unbalanced optimal transport](https://github.com/thibsej/unbalanced_gromov_wasserstein)  
**2)** Unsupervised hyperparameter tuning  
When missing correspondence information for performing hyperparameter selection, SCOT uses Gromov-Wasserstein distance as an approximation for alignment quality.  
**3)** Switch to correlation (from Euclidean distance) as a distance metric for kNN graphs  
**4)** Switch to connectivity (from distance) for kNN graph edge annotations  

**Python packages required:**
numpy, sklearn, matplotlib, scipy, cython, POT (note that numpy and cython must be installed prior to POT)
