![plot](inst/epiregulon_logo.png)<br>

# Introduction

Gene regulatory networks model the underlying gene regulation hierarchies that drive gene expression and cell states. The main function of the epiregulon package is to construct gene regulatory networks and infer transcription factor (TF) activity in single cells by integration of scATAC-seq and scRNA-seq data and incorporation of public bulk TF ChIP-seq data.

For full documentation, please refer to the epiregulon [book](https://xiaosaiyao.github.io/epiregulon.book/).

Preprint
Epiregulon: Inference of single-cell transcription factor activity to dissect mechanisms of lineage plasticity and drug response
Tomasz Wlodarczyk, Aaron Lun, Diana Wu, Shreya Menon, Shushan Toneyan, Kerstin Seidel, Liang Wang, Jenille Tan, Shang-Yang Chen, Timothy Keyes, Aleksander Chlebowski, Yu Guo, Ciara Metcalfe, Marc Hafner, Christian W. Siebel, M. Ryan Corces, Robert Yauch, Shiqi Xie, Xiaosai Yao
bioRxiv 2023.11.27.568955; doi: [https://doi.org/10.1101/2023.11.27.568955](https://www.biorxiv.org/content/10.1101/2023.11.27.568955v1)

![plot](inst/epiregulon_schematics.svg) 
There are three related packages. The core epiregulon package supports `SingleCellExperiment` objects. If the users would like to start from `ArchR` projects, they may choose to use `epiregulon.archr` package, which allows for the seamless integration with the [ArchR](https://www.archrproject.com/) package. Moreover, we provide a suite of tools in `epiregulon.extra` package for the enrichment analysis, visualization, and network analysis which can be run on the `epireglon` or `epiregulon.archr` output.

# Installation

```
# install devtools
if(!require(devtools)) install.packages("devtools")

# install basic epiregulon package
devtools::install_github(repo='xiaosaiyao/epiregulon')

# install extended version of epiregulon
devtools::install_github(repo='xiaosaiyao/epiregulon.archr')

# install extended version of epiregulon
devtools::install_github(repo='xiaosaiyao/epiregulon.extra')
```

Example data included in the tutorial are available from [scMultiome](https://bioconductor.org/packages/release/data/experiment/html/scMultiome.html) 

```
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("scMultiome")
```

# Functions
Functions in the suite of Epiregulon packages
![plot](inst/epiregulon_functions.png)


Contact: [Xiaosai Yao](mailto:yao.xiaosai@gene.com), Genentech Inc.


