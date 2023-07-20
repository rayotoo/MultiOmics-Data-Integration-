# MultiOmics-Data-Integration-
# Resources
# Main Tutorial
```
https://nbisweden.github.io/workshop_omicsint_ISMBECCB/schedule.html
```
# 1. Supervised OMICs Integration
```
https://nbisweden.github.io/workshop_omicsint_ISMBECCB/session_ml/SupervisedOMICsIntegration/supervised_omics_integr_CLL.html
```

This script performs data integration of proteomics, DNA methylation, and RNA-seq data using the mixOmics package in R. The integration analysis considers two factors: sex (males and females) and treatment (sham and IR). It aims to identify shared patterns and relationships across the different omics datasets.

# Prerequisites
R: Ensure that R and the required packages are installed. You can install the required packages by running the following command in R:
```
install.packages(c("mixOmics"))
```


# Usage

1. Prepare your data:

+ Organize your proteomics, DNA methylation, and RNA-seq data in separate tables, with samples as rows and variables (e.g., proteins, methylation sites, gene expression levels) as columns.
+ Ensure that the samples are in the same order across the three datasets, so that they can be correctly matched during the integration process.
2. Open the integration_script.R file and update the following variables:

+ proteomicsData: Path to the proteomics data file.
+ methylationData: Path to the DNA methylation data file.
+ rnaSeqData: Path to the RNA-seq data file.

3. Run the script:
+ Execute the integration_script.R file in R or RStudio.
  
4. Interpret the results:

+ The script will perform data integration using mixOmics and generate performance metrics and plots to explore the integrated results.
+ Refer to the generated plots and metrics to interpret the integration analysis.

# Results
The script will generate the following results:

+ Performance Metrics: The script will calculate performance metrics, such as classification accuracy and stability measures, to assess the quality of the data integration model.

+ Plots:

   + Individual Sample Plot: A scatter plot of the integrated samples, visualizing the relationship between the two components (latent variables) and colored by sex and treatment.
   + Variable Importance Plot: A bar plot showing the importance of variables (e.g., proteins, methylation sites, gene expression levels) in the data integration analysis.
