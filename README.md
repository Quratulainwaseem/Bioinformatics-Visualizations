# Bioinformatics-Visualizations

A collection of publication-ready bioinformatics figures generated in R — covering gene ontology enrichment, miRNA-mRNA network plots, and expression analysis visualizations.

---

## Overview

This repository contains reusable R scripts for generating high-quality figures commonly used in genomics and transcriptomics research. All plots are designed to meet journal submission standards and are fully customizable.

---

## Figures Included

### 1. GO Enrichment Plots
Barplots for Gene Ontology enrichment across three categories:
- **Biological Process (BP)**
- **Cellular Component (CC)**
- **Molecular Function (MF)**

### 2. miRNA–mRNA Interaction Network
Cytoscape-generated network visualization showing miRNA-mRNA regulatory relationships in Small Cell Lung Cancer (SCLC).

### 3. Differential Expression Outputs
Visual summaries of differentially expressed miRNAs between tumor and normal tissue.

---

## Repository Structure

```
Bioinformatics-Visualizations/
├── scripts/
│   ├── GO_enrichment_plots.R       # GO barplots (BP, CC, MF)
│   ├── network_visualization.R     # Cytoscape network export
│   └── DEG_visualization.R        # Volcano plot, heatmap
├── figures/
│   ├── GO_BP_barplot.png
│   ├── GO_CC_barplot.png
│   ├── GO_MF_barplot.png
│   └── Cytoscape_miRNA_mRNA_network.png
└── README.md
```

---

## Sample Figures

### GO Biological Process
![GO BP](figures/GO_BP_barplot.png)

### GO Cellular Component
![GO CC](figures/GO_CC_barplot.png)

### GO Molecular Function
![GO MF](figures/GO_MF_barplot.png)

### miRNA–mRNA Network
![Network](figures/Cytoscape_miRNA_mRNA_network.png)

---

## Tools & R Packages

| Package | Purpose |
|---------|---------|
| `ggplot2` | Core plotting |
| `clusterProfiler` | GO & KEGG enrichment |
| `enrichplot` | Enrichment visualization |
| `org.Hs.eg.db` | Human gene annotation |
| `dplyr` | Data wrangling |

---

## Requirements

```r
install.packages(c("ggplot2", "dplyr"))

if (!requireNamespace("BiocManager", quietly = TRUE))
  install.packages("BiocManager")

BiocManager::install(c("clusterProfiler", "enrichplot", "org.Hs.eg.db"))
```

---

## How to Use

1. Clone this repository
2. Install required packages (see above)
3. Open any script in `/scripts/`
4. Replace input data path with your own dataset
5. Run script — figures save automatically to `/figures/`

---

## Author

**Quratulain Waseem**
MS Computational Biotechnology — Gold Medalist
University of Management and Technology, Sialkot, Pakistan

- LinkedIn: [quratulain-waseem-239310353](https://www.linkedin.com/in/quratulain-waseem-239310353)
- ORCID: [0009-0003-9735-5632](https://orcid.org/0009-0003-9735-5632)

---

> Scripts are generalized and can be applied to any RNA-seq or miRNA expression dataset.
