

## [Single site annotation](https://github.com/BioInfoData/single_site_annotation)

Provides full annotation for list of sites in a single base resolution.

The annotation includes: 

* General annotation: Ensembl gene ID;  Ensembl trenscript ID; biotype; gene symbol; HID.
* Position in the transcript (for sites within genes): exon/ intron ;  5UTR/ 3UTR/ CDS;  position of the site within the transcript relative to TSS.
* Translation information (for siteses within CDS):  amino acid name; coding frame of the site; codon sequence.
* Metagene plots of all input sites.

**Language: Python3**

**Tools: bedtools**

**Required moduls: pybedtools, pandas, numpy, biopython, matplotlib**

![pic2](https://user-images.githubusercontent.com/93220699/183313469-d1b6086c-27c0-41ba-ba84-b2b26ffc9a65.png)




