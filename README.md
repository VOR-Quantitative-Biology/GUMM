
![Scheme](images/GUMM_RW.png)

---
## GUMM: Genotyping Using Mixture Models

This R package interfaces with [CRISPResso2](https://github.com/pinellolab/CRISPResso2)'s allele count summary output to perform automatic genotyping of CRISPR-Cas9 editing events from single cell DNAseq data. It applies a series of mixture models to analyze cell allele frequencies, ploidy, and allele co-occurrence to genotype and detect doublets without the need to set arbitrary cutoffs. The method does not require multiple loci to identify doublets and relies only on allele frequencies from a single edited site. This makes GUMM well-suited to analyze genetically homogeneous cell samples where cells have been edited at only one loci (assuming negligible off targets). Furthermore, the package can rapidly genotype thousands of cells within minutes.

### Installation
**1. Install package using remotes**
```sh
remotes::install_bitbucket("vor-compbio/GUMM")
```
<br/>
**2. Load package in R**
```sh
library(GUMM)
```
<br/><br/><br/>
If publishing research using GUMM, please cite this [preprint](https://www.biorxiv.org/content/10.1101/2025.05.22.653824v1)
