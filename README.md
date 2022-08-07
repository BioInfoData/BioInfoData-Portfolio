

# [Single site annotation](https://github.com/BioInfoData/single_site_annotation)

Provides full annotation for list of sites in a single base resolution.

The annotation includes: 

* General annotation: Ensembl gene ID;  Ensembl trenscript ID; biotype; gene symbol; HID.
* Position in the transcript (for sites within genes): exon/ intron ;  5UTR/ 3UTR/ CDS;  position of the site within the transcript relative to TSS.
* Translation information (for siteses within CDS):  amino acid name; coding frame of the site; codon sequence.
* Metagene plots of all input sites.

**Language: Python3**

**Required tools: bedtools**

**Required moduls: pybedtools, pandas, numpy, biopython, matplotlib**

![pic2](https://user-images.githubusercontent.com/93220699/183313469-d1b6086c-27c0-41ba-ba84-b2b26ffc9a65.png)



# [Strand specific pileup for RNAseq](https://github.com/BioInfoData/pileup_stranded)

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
