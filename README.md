# BioInfoData Portfolio

<h3><a href="#web">Web Development: NGS tools review for beginners (Python - Django, html, css)</a></h3>
<h3><a href="#pileup">NGS Tool Development: Strand specific pileup for RNAseq (Python)</a></h3>
<h3><a href="#anot">NGS Tool Development: Single site annotation (Python)</a></h3>
<h3><a href="#coverage">NGS Tool Development: Mean coverage plot for list of sites (Python)</a></h3>
<h3><a href="#cluster">Data Analysis: Find micro-clusters in 2D gene expression data (R)</a></h3>
<h3><a href="#spots">Data Analysis: Analysis of gene expression pattern in 2D space (R)</a></h3>

<h1>Overview</h1>

<p id = "web"></p>

## [Web Development: NGS tools review for beginners](http://bioinfodata.eu.pythonanywhere.com/)

A website that summarizes the most useful tools for bioinformatic analysis of Next Generation Sequencing (NGS).

**Language: Python3, Html, CSS**

**Required moduls: Django, Pillow**

<img src="https://user-images.githubusercontent.com/93220699/188962869-097f71c2-ec9d-4a3f-8cce-864d786073bd.png" alt="drawing" width="800"/>

<p id = "pileup"></p>

## [NGS Tool Development: Strand specific pileup for RNAseq](https://github.com/BioInfoData/pileup_stranded)

A common task in bioinformatics is pileup of alignment files for detecting muation, inserstion or deletions sites.

The current tool provide a site specific pileup with the following advantages comparing to other tools:

* Using **mutliproccesing** to decreas the time of analysis.

* Allow **strand specific pileup** for RNA-seq data.

* Allow **selection of specific nucleotides** to include in the analysis in order to decres the runing time and size of output files.

* Allow **filtering of the results** based on coverate, muation rate or number of mutated reads.

* Allow **pileup only for list of sites** provided as input file to the tool.

**Language: Python3**

**Required tools: samtools**

**Required moduls: pysam, pandas, biopython**

[View on GitHub](https://github.com/BioInfoData/pileup_stranded)

<p id = "anot"></p>

## [NGS Tool Development: Single site annotation](https://github.com/BioInfoData/single_site_annotation)

Provides full annotation for list of sites in a single base resolution.

The annotation includes: 

* General annotation: Ensembl gene ID;  Ensembl trenscript ID; biotype; gene symbol; HID.

* Position in the transcript (for sites within genes): exon/ intron ;  5UTR/ 3UTR/ CDS;  position of the site within the transcript relative to TSS.

* Translation information (for siteses within CDS):  amino acid name; coding frame of the site; codon sequence.

* Metagene plots of all input sites.

**Language: Python3**

**Required tools: bedtools**

**Required moduls: pybedtools, pandas, numpy, biopython, matplotlib**

[View on GitHub](https://github.com/BioInfoData/single_site_annotation)

<img src="https://user-images.githubusercontent.com/93220699/183313469-d1b6086c-27c0-41ba-ba84-b2b26ffc9a65.png" alt="drawing" width="500"/>

<p id = "coverage"></p>

## [NGS Tool Development: Mean coverage plot for list of sites](https://github.com/BioInfoData/metasite_coverage)

This tool execpts BAM file and a list of sites in bed6 format and generates mean coverage plot around the sites.

**Language: Python3**

**Required tools: samtools**

**Required moduls: pysam, pandas, numpy, matplotlib**

[View on GitHub](https://github.com/BioInfoData/metasite_coverage)

<img src="https://user-images.githubusercontent.com/93220699/183314555-91a9ed91-6851-4669-932c-b326e4023dc1.png" alt="drawing" width="500"/>

<p id="cluster"></p>

## [Data Analysis: Find micro-clusters in 2D gene expression data](https://github.com/BioInfoData/find_clusters) 

The goal of this analysis is to test whether there is micro organization of cells in a way that neighboring nerunal cells will be more likely to express same IEG gene following stimulation resluting with "micro-clusters". 

At the fisrt step of the analysis we calculate the probability of a cells being an IEG positive cell as a function of its distance from other IEG positive cell.

In the second step of analysis we will try to find “cluster” of positive cells. We will start from a positive cell recursively add cells to this cluster as long as they are located less then 20 micron and that at least 80% of the cells in the environment are positive.

The data used for the analysis is smFISH experiment results and the analysis was part of [this](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7519336/pdf/pnas.201913658.pdf) publication.

**Language: R**

**Libraries: ggplot2, raster**

[View on GitHub](https://github.com/BioInfoData/find_clusters) 

<img src="https://user-images.githubusercontent.com/93220699/183497766-8958b975-156f-4520-9daa-57fc1c867e08.png" alt="drawing" width="800"/>

<p id = "spots"></p>

## [Data Analysis: Analysis of gene expression pattern in 2D space](https://github.com/BioInfoData/find_hotspot)

Demonstration of spacial data analysis in order to find "hotspots" of expression in mouse brain sections. 

The data used for the analysis is smFISH experiment results and the analysis was part of [this](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7519336/pdf/pnas.201913658.pdf) publication.


**Language: R**

**Libraries: ggplot2, mgcv, dplyr, permute**

[View on GitHub](https://github.com/BioInfoData/find_hotspot)

<img src="https://user-images.githubusercontent.com/93220699/183315614-81488be7-6a6f-4d4a-adab-4b3c0c6904d2.png" alt="drawing" width="500"/>

