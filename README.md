# Phylogeny analysis for herpesvirus glycoproteins

This repo contains multiple directories that analyze the diversity of specific herpesvirus glycoproteins by running a [snakemake](https://snakemake.readthedocs.io/) pipeline that downloads sequences based a list of accessions, processes the sequences, and constructs a phylogenetic Nextstrain tree that can be viewed using [Auspice](https://auspice.us/). Each herpesvirus directory contains its own snakemake pipeline. 

**The numbering scheme of each protein is relative to the [NCBI Virus](https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/) reference strains (***HSV-1: NC_001806.2, EBV: NC_007605.1, HSV-2: NC_001798.2***).**

Analysis performed by Caleb Carr.

## Nextstrain visualizations of the trees

**The tree can be colored by several features (e.g., genotype, date, country) by selecting the corresponding option in the ***Color By*** dropdown. For example, the [HSV-1 gB tree](HSV1/Results/HSV1_gB/Alignments/protein_ungapped_no_outgroup.fasta) can be colored by amino acid identity at a position by selecting ***Genotype*** in the dropdown menu and then selecting ***HSV1_gB***. Entering a position will then color the tree by the amino acid identity at that position. Note that the protein numbering is relative to the [NCBI Virus](https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/) reference strains (***HSV-1: NC_001806.2, EBV: NC_007605.1, HSV-2: NC_001798.2***). Other features can be viewed by mousing over or clicking on the nodes and branches of the tree.**

HSV-1: 
- [glycoprotein B](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV1/gB)
- [glycoprotein D](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV1/gD)
- [glycoprotein H](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV1/gH)
- [glycoprotein L](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV1/gL)

EBV: 
- [glycoprotein B](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/EBV/gB)
- [glycoprotein 42](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/EBV/gp42)
- [glycoprotein H](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/EBV/gH)
- [glycoprotein L](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/EBV/gL)

HSV-2: 
- [glycoprotein B](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV2/gB)
- [glycoprotein D](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV2/gD)
- [glycoprotein H](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV2/gH)
- [glycoprotein L](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV2/gL)

## Protein alignments of glycoproteins

**Alignments are constructed relative to the [NCBI Virus](https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/) reference strains (***HSV-1: NC_001806.2, EBV: NC_007605.1, HSV-2: NC_001798.2***).**

HSV-1: 
- [glycoprotein B](HSV1/Results/HSV1_gB/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein D](HSV1/Results/HSV1_gD/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein H](HSV1/Results/HSV1_gH/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein L](HSV1/Results/HSV1_gL/Alignments/protein_ungapped_no_outgroup.fasta)

EBV: 
- [glycoprotein B](EBV/Results/EBV_gB/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein 42](EBV/Results/EBV_gp42/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein H](EBV/Results/EBV_gH/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein L](EBV/Results/EBV_gL/Alignments/protein_ungapped_no_outgroup.fasta)

HSV-2: 
- [glycoprotein B](HSV2/Results/HSV2_gB/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein D](HSV2/Results/HSV2_gD/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein H](HSV2/Results/HSV2_gH/Alignments/protein_ungapped_no_outgroup.fasta)
- [glycoprotein L](HSV2/Results/HSV2_gL/Alignments/protein_ungapped_no_outgroup.fasta)

## Organization of this repo

- [`HSV1`](HSV1/): Contains the analysis workflow for HSV-1
- [`EBV`](EBV/): Contains the analysis workflow for EBV
- [`HSV2`](HSV2/): Contains the analysis workflow for HSV-2
- [`auspice`](auspice/): Contains the final nextstrain tree files for each herpesvirus that then can be viewed using [Nextstrain community share via GitHub](https://docs.nextstrain.org/en/latest/guides/share/community-builds.html). **Note that these final files are manually copied from each individual herpesvirus directory.**