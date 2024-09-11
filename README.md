# Phylogeny analysis for herpesvirus glycoproteins

This repo contains multiple directories that analyze the diversity of specific herpesvirus glycoproteins by running a [snakemake](https://snakemake.readthedocs.io/) pipeline that downloads sequences based a list of accessions, processes the sequences, and constructs a phylogenetic Nextstrain tree that can be viewed using [Auspice](https://auspice.us/). Each herpesvirus directory contains its own snakemake pipeline. 

Analysis performed by Caleb Carr.

## Nextstrain visualizations of the trees

- HSV1 [https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV1/gB](https://nextstrain.org/community/jbloomlab/Herpesvirus-Glycoprotein-Analysis/HSV1/gB)

## Organization of this repo

- [`HSV1`](HSV1/): Contains the analysis workflow for HSV-1
- [`auspice`](auspice/): Contains the final nextstrain tree files for each herpesvirus that then can be viewed using [Nextstrain community share via GitHub](https://docs.nextstrain.org/en/latest/guides/share/community-builds.html). Note that these final files are manually copied from each individual herpesvirus directory.