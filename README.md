# Brendo
Open resource for uniquely transcribed genes in brain endothelial cells

<img  src="https://github.com/CompGenomeLab/brendo/blob/dev/home_banner.png"/>

## Table of Contents
* [Overview](#overview)
* [Contents](#repocontents)
	* [Directory Structure](#dirstructure)


## Overview <a name="overview"></a>

The blood-brain barrier (BBB) plays a critical role in central nervous system homeostasis, yet comprehensive transcriptional profiling of brain microvascular endothelial cells (BMECs) remains limited. Leveraging the increasing availability of publicly accessible bulk RNA sequencing (RNA-seq) datasets, we
developed an integrated analytical framework to identify genes selectively enriched in BMECs compared to endothelial cells (ECs) from other tissues. To address the substantial batch effects inherent to multi-source bulk RNA-seq data, we combined two differential expression strategies, rank aggregation methods, and extensive quality controls. Our analysis incorporated EC samples from 16 different tissues and employed robust statistical workflows to mitigate technical confounders while preserving biologically meaningful signals. Validation using known BBB markers and independent proteomic evidence confirmed the reliability of our approach. We present Brendo (Brain Endothelial Open Resource), an open-access web platform providing searchable, filterable, and downloadable data on differentially expressed genes in BMECs. Brendo enables an in-depth exploration of brain endothelial gene expression and offers broader applications across vascular biology by supporting cross-tissue EC comparisons.

## Contents <a name="repocontents"></a>

This repository contains scripts required to reproduce the analysis, as well as code required to run Brendo locally / set up a copy of Brendo. See the subdirectories for detailed instructions. For a deployed version of Brendo, click <a href="https://brendo.sabanciuniv.edu"> here </a>.


###  Directory Structure <a name="dirstructure"></a>
```bash
root
├── Alignment  # Includes Snakemake pipeline used for alignment / quantification
│	├── bin  # Includes scripts ran through Snakemake
│   └── Modules  # Includes Snakemake rules to be ran  
│	    ├── Align  # Alignment rules
│       ├── GetCounts  # Quantification rules
│       └── SRActions  # Read file download rules
│
└── Server  # Includes content required to run the web applicaiton
	├── FastAPI (Data) # API requirements
	└── ReactJS (Webpage)  # Webpage requirements
```
