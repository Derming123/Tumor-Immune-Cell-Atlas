# Breast Invasive Ductal Carcinoma

## Data description
This data corresponds to 2 serial breast carcinoma sections and comes from the 10x Genomics website with the following definition: 

*10x Genomics obtained fresh frozen Invasive Ductal Carcinoma breast tissue from BioIVT Asterand. The tissue was embedded and cryosectioned as described in Visium Spatial Protocols - Tissue Preparation Guide (Demonstrated Protocol CG000240). Tissue sections of 10 µm thickness were placed on Visium Gene Expression Slides.*

*The tissue was AJCC/UICC Stage Group IIA, ER positive, PR negative, Her2 positive and annotated with:*
- *Ductal carcinoma in situ*
- *Lobular carcinoma in situ*
- *Invasive Carcinoma*

## Data availability
This data is freely available to download from the 10X Genomics website reference datasets and can be downloaded directly from their website - Slice 1 is available [here](https://support.10xgenomics.com/spatial-gene-expression/datasets/1.0.0/V1_Breast_Cancer_Block_A_Section_1) and Slice 2 [here](https://support.10xgenomics.com/spatial-gene-expression/datasets/1.0.0/V1_Breast_Cancer_Block_A_Section_2).
In this case we are using the data mapped using spaceranger 1.0.0.

## Code
Scripts *1-10x_breast_QC.Rmd* and *2-10x_breast_GO_enrichment.Rmd* are in charge of preprocessing the data and mapping the TCA immune cell states onto the tissue. 
Scripts *3-10x_breast_immune_reference.Rmd*  and *4-10x_breast_stratification.Rmd*, in turn, plot the Figure panels of Figure 6 and Supplementary Figure 13-17.

## Dependencies
* [R 3.6.0](https://cran.r-project.org/)
* [Seurat 3.2.0](https://cran.r-project.org/web/packages/Seurat/index.html)
* [tidyverse 1.3.0](https://cran.r-project.org/web/packages/tidyverse/index.html)
* [ggpubr 0.3.0](https://cran.r-project.org/web/packages/ggpubr/index.html)
* [SPOTlight 1.0.0](https://github.com/MarcElosua/SPOTlight)
* [Matrix 1.2.18](https://cran.r-project.org/web/packages/Matrix/index.html)
* [svglite 1.2.3.2](https://cran.r-project.org/web/packages/svglite/index.html)
* [ggcorrplot 0.1.3](https://cran.r-project.org/web/packages/ggcorrplot/index.html)
* [cowplot 1.1.0](https://cran.r-project.org/web/packages/cowplot/index.html)

