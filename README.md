# Raw qPCR eDNA data for Chondria tumulosa detection at Majuro, RMI
[![DOI](https://zenodo.org/badge/1054827145.svg)](https://doi.org/10.5281/zenodo.17099779)

Nichols, P., et al. (2025). 

This repository contains raw and processed environmental DNA (eDNA) data, along with R scripts for data processing, analysis, and figure generation, associated with the detection of Chondria tumulosa at Majuro, Republic of the Marshall Islands (RMI). These data support the analyses presented in Nichols et al., 2025 (submitted to Biology Letters). The dataset includes:

* Raw qPCR eDNA results for Chondria detection (.csv).
* Quantitative amplification and cycle threshold (Cq) data (.csv).
* Long-read sequence data from ONT MinION sequencing (.fastq.gz).
* Blastn search results for sequence assignment (.csv).
* R scripts for processing qPCR results and generating figures (.rmd).

## Quantitative PCR (qPCR) data includes:

* **quantification amplification results (Quantification_Amplification_Results_SYBR.csv)** - raw qPCR data includes project ID, cycle number, relative fluorescence units (value), sample date, sample region, site ID, latitude, longitude, filtration method (active or passive), island/atoll, and plate well ID

* **quantification Cq results for passive methods (Quantification_Cq_Results_SYBR.csv)** - raw qPCR detection and quantification data includes project ID, plate well ID, fluorescent marker ("SYBR"), quantification cycle (Cq.Mean), log starting quantity (Log.Starting.Quantity), mean starting quantity (SQ.Mean), assay annealing temperature (Set.Point), sample ID, sample number, sample date, sample region, site ID, latitude, longitude, filtration method, visual detection (presence-absence), island/atoll, replicate number, qPCR detection (presence-absence)

## Long-read eDNA sequence data includes:

* **Raw sequence data (ONT_MINION_raw.fastq)** - raw sequence reads generated from ONT Minion single sequencing run

* **Blastn query hit table (ONT_MINION_blastn_table.csv)** - resulting data from NCBI blastn search of the nucleotide database includes molecular operational taxonomic unit identifiers (MOTU_ID), read number (reads), proportion of assigned reads (prop), taxonomic match (organism), sequence pairwise match (% Pairwise Identity), accession number (Accession), bit-score, e-value, query coverage (%), length (bp), grade (%), and sequence

## Scripts:
R scripts for processing qPCR data and generating figures are included in the /R_scripts folder. Scripts require R version ≥4.2.0.

## Citation
Please cite the associated manuscript when using these data.
