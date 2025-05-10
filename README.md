# Sample Teaching Resources

This repository showcases selected teaching materials developed by Dr. Fan Wang for university-level courses in statistics and genomics. 

We provide a toy dataset in [example](/example). 
The input data includes 
1) the binary genotype file in [example](/example) contains N sample = 500 individuals (column "IID") 
and N variant = 100 SNPs from the [https://github.com/cloufield/GWASTutorial.git/01_Dataset/download_sampledata.sh](https://github.com/cloufield/GWASTutorial.git/01_Dataset/download_sampledata.sh).
2) the [phenotype file](example/normalized_pheno.txt) that contains one simulated quantitative trait (column "Y1") for the N sample = 500 individuals (column "IID").
3) the [covariate file](example/covariate.txt) that contains two simulated covariates (columns "covar1" and "covar2") for the N sample = 500 individuals (column "IID").

Run the R script [example.regenie.qrs.R](/example/example.regenie.qrs.R) to perform Regenie.QRS (single variant tests) for the phenotype and genotype data in [example](/example). Set ```is.effect.estimated = T``` to enable the estimation of quantile-specific effect size (disabled by default). Set ```data.path``` to the directory where you store your data and results, and set ```Regenie.path``` to the location where the Regenie executable is installed.
