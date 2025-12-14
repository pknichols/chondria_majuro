# Raw qPCR eDNA data for Chondria tumulosa detection at Majuro, RMI
[![DOI](https://zenodo.org/badge/1054827145.svg)](https://doi.org/10.5281/zenodo.17099779)

Nichols PK, Fumo JT, Lopes Jr. KH, Ely TD, Nash EN, Timmers MA, Sherwood AR, Marko PB (2025). When cryptogenic species are also cryptic: reframing biogeographic uncertainty in the eDNA era. _Biology Letters_ 

This repository contains raw environmental DNA (eDNA) qPCR and sequence data, along with R scripts for data analysis associated with the detection of _Chondria tumulosa_ at Majuro, Republic of the Marshall Islands (RMI). The dataset includes:

* Raw qPCR amplification curve results (.csv) from _in situ_ eDNA screening.
* Raw qPCR cycle threshold (Cq) data (.csv) from _in situ_ eDNA screening.
* Long-read sequence Oxford Nanopore (ONT) MinION sequences (.fastq.gz) generated from initial detection among pooled RMI samples.
* Blastn search results from ONT sequence assignment (.csv).
* R scripts for processing and visualizing qPCR results (.rmd).

## Quantitative PCR (qPCR) data includes:

* **quantification amplification results (Quantification_Amplification_Results_SYBR.csv)** - raw qPCR data includes project sample unique ID (ID), qPCR cycle number (Cycle), relative fluorescence units (value), sample date (Date), sample region (Region), site (Site_ID), latitude, longitude, filtration method (active or passive), island/atoll (Atoll), and 96-well plate location map (PlateID)

* **quantification Cq results for passive methods (Quantification_Cq_Results_SYBR.csv)** - raw qPCR detection and quantification data includes project sample unique ID (ID), 96-well plate location map (Well), fluorescent marker (Fluor), quantification cycle Cq-value (Cq.Mean), log starting quantity target DNA concentration per uL (Log.Starting.Quantity), mean starting quantity target DNA concentration per uL (SQ.Mean), assay annealing temperature in degrees Celsius (Set.Point), biological replocate sample number (Sample), sample date (Date), sample region (Region), site (Site_ID), latitude, longitude, filtration method, visual detection presence-absence (Visual), island/atoll (Atoll), qPCR technical replicate number (Replicate), qPCR detection presence-absence (qPCR_presence)

## Sequence data includes:

* **Raw sequence data (ONT_MINION_raw.fastq)** - raw sequence reads generated from ONT Minion single sequencing run of positive pooled sample qPCR amplicons

* **Blastn query hit table (ONT_MINION_blastn_table.csv)** - resulting data from NCBI blastn search of the nucleotide database includes molecular operational taxonomic unit unique identifiers (MOTU_ID), read number (reads), proportion of assigned reads (prop), taxonomic match (Organism), sequence pairwise match (% Pairwise Identity), accession number (Accession), bit-score, e-value, query coverage (%), length (bp), grade (%), and MOTU sequence (Sequence)

*  **Sequence Alignment (.fasta) files** - MAFFT sequence alignments for each loci (COI, rbcL, SSU, UPA) that were used to generate separate consensus trees with IQ-TREE v1.6.12

## Scripts:
R scripts are included and require R version ≥4.2.0. Package versions are documented via `sessionInfo()` at the end of the R Markdown file.

To reproduce the analysis:
1. Clone or download this repository
2. Open `/CTmajuro.Rmd`
3. Knit the document in RStudio

## Citation
Please cite the associated manuscript when using these data.

## License
This repository is licensed under a Creative Commons Attribution 4.0 International License (CC BY 4.0).  
See the LICENSE file for details.
