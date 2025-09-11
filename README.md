# chondria_majuro
 Raw qPCR eDNA data for Chondria detection at Majuro, RMI

## Quantitative PCR (qPCR) data includes:

* **quantification amplification results (Quantification_Amplification_Results_SYBR.csv)** - raw qPCR data includes project ID, cycle number, relative fluorescence units (value), sample date, sample region, site ID, latitude, longitude, filtration method (active or passive), island/atoll, and plate well ID

* **quantification Cq results for passive methods (Quantification_Cq_Results_SYBR.csv)** - raw qPCR detection and quantification data includes project ID, plate well ID, fluorescent marker ("SYBR"), quantification cycle (Cq.Mean), log starting quantity (Log.Starting.Quantity), mean starting quantity (SQ.Mean), assay annealing temperature (Set.Point), sample ID, sample number, sample date, sample region, site ID, latitude, longitude, filtration method, visual detection (presence-absence), island/atoll, replicate number, qPCR detection (presence-absence)

## Long-read eDNA sequence data includes:

* **Raw sequence data (ONT_MINION_raw.fastq)** - raw sequence reads generated from ONT Minion single sequencing run

* **Blastn query hit table (ONT_MINION_blastn_table.csv)** - resulting data from NCBI blastn search of the nucleotide database includes molecular operational taxonomic unit identifiers (MOTU_ID), read number (reads), proportion of assigned reads (prop), taxonomic match (organism), sequence pairwise match (% Pairwise Identity), accession number (Accession), bit-score, e-value, query coverage (%), length (bp), grade (%), and sequence

[![DOI](https://zenodo.org/badge/1054827145.svg)](https://doi.org/10.5281/zenodo.17099779)
