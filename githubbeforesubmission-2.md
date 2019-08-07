Sara Saez-Atienzar, Sara Bandres-Ciga, Mike Nalls.
 
March 2019

# ALS_Pathway analysis based on Polygenic Risk Scores 

## Introduction
Despite the considerable progress made in unraveling the genetic causes of amyotrophic lateral sclerosis (ALS), we do not fully understand the molecular mechanisms underlying the disease. We analyzed genome-wide data involving nearly 80,000 individuals using a polygenic risk score approach to identify the biological pathways and cell types involved in ALS.
## Overview
We have performed a **three-stage study design** to identify pathways and cell types relevant to ALS risk

**Reference Dataset.** A published GWAS study involving 12,577 ALS cases and 23,475 controls (*Van Rheenen et al., 2016*)
https://www.ncbi.nlm.nih.gov/pubmed/27455348
The summary statistics is used to define risk allele weights for the construction of polygenic risk scores.

**Training Dataset**. 	Plink Binary files containing individual-level data  genotype in our lab and  consisting in 5,653 ALS cases and 24,629 control subjects that were genotyped in our laboratory *(Nicolas et al., 2018)*.
https://www.ncbi.nlm.nih.gov/pubmed/29566793
The regression models generated from the reference data is used to construct and test polygenic risk scores within the training data. 

**Replication Dataset.** Plink Binary files containing individual-level data  genotype in our lab and  consisting in  2,420 ALS cases and 10,555 controls genotyped in our laboratory*(Nicolas et al., 2018)*.
https://www.ncbi.nlm.nih.gov/pubmed/29566793


# Pathway analysis based on Polygenic Risk Scores using PRSice-2

A detailed information can be found in the following link:
https://choishingwan.github.io/PRSice/

###### Citation: PRSice: Polygenic Risk Score software, Euesden, Lewis, O'Reilly, Bioinformatics (2015) 31 (9):1466-1468

## Requirements

#### PRSice2_Linux executable (v2.2)
#### PLINK binary files with PCAs and a covariate file. Due to the nature of PRS analysis, it is recommendable to include 20 PCs

#### [R](https://www.r-project.org/) (**version 3.2.3+**)

#### PRSet Specific Input


-   **MSigDB file**: File containing name of each gene sets and the ID of genes within the gene set on each individual line. If MSigDB is provided, GTF file is required.
-   **GTF file**: A file contain the genome boundary of each individual gene


## Base file
Summary Stats without overlapping samples with training dataset. We have used a previous published GWAS summary Stats (Van Rheenen et al., 2016) https://www.ncbi.nlm.nih.gov/pubmed/27455348

## Training file
Training dataset: Raw genotype data of "target phenotype" in the form of PLINK binary
https://www.ncbi.nlm.nih.gov/pubmed/29566793

## Replication file: Raw genotype data of "target phenotype" in the form of PLINK binary
https://www.ncbi.nlm.nih.gov/pubmed/29566793


# CODE for training
Coming by September.

# CODE for Replication

Coming by September.
