# Supplementary Material
The code provided by this repository is part of the supplementary material for the scientific article "In Vitro and In Vivo Toxicometabolomics of the Synthetic Cathinone PCYP Studied by Means of LC-HRMS/MS" by Selina Hemmer et al., Metabolites, 2022 (<DOI:10.3390/metabo12121209>). See the following sections for detailed information about it. Corresponding files can be found at MetaboLights using the study identifier MTBLS6469.

# Source Code

## Dependencies

The code deployed by this repository requires the following packages:

-   tidyverse (CRAN)
-   ggrepel (CRAN)
-   gplots (CRAN)
-   MASS (CRAN)
-   caret (CRAN)
-   XCMS (Bioconductor)
-   CAMERA (Bioconductor)

If not installed you can use the following lines to install them:

     `install.packages(c("tidyverse", "ggrepel", "gplots", "MASS", "caret")
     source("https://bioconductor.org/biocLite.R")
     biocLite(c("xcms", "CAMERA"))`

Additionally, evaluation script require functions provided by the metaboLib.R library. The corresponding library can be found [here](https://github.com/saskema/metaboLib).

## Usage

To use the scripts as deployed in this repository, place the matching script in the same folder were the files are grouped in folders corresponding to their study group (e.g. "Blank", "PCYP", "QC") and run it.

## Result

You will obtain the following files:

-   evaluateResults/sampleStatistics.pdf
-   evaluateResults/evaluate.RData
-   evaluateResults/Chromatogram.pdf
-   evaluateResults/peaklistCAMERA.csv
-   evaluateResults/significant_results.csv

### pHLM

Contains the scripts used for pooled human liver microsome (pHLM) samples. Scripts were used to evaluate the sample analyses by performing peak picking and subsequent staistical analysis. The suffixes "pos" and "neg" describe their usage for each ionization mode.

### Rat_plasma

Scripts were used to evaluate the sample analyses by performing peak picking and subsequent staistical analysis.Contains the scrips used for rat plasma samples. Scripts that contain "PH" in their name describe their usage for Phenylhexyl column. Scripts that contain "ZicHILIC" in their name describe their usage for ZicHILIC column. The suffixes "pos" and "neg" describe their usage for each ionization mode.

### Rat_urine

Scripts were used to evaluate the sample analyses by performing peak picking and subsequent staistical analysis. Contains the scrips used for rat urine samples. Scripts that contain "PH" in their name describe their usage for Phenylhexyl column. Scripts that contain "ZicHILIC" in their name describe their usage for ZicHILIC column. The suffixes "pos" and "neg" describe their usage for each ionization mode.

## centWaveOpt.R

### General

This script was used to perform peak picking optimization according to <DOI:10.1002/dta.2552>.
