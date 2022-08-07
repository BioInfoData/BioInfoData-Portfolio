

## [Single site annotation](https://github.com/BioInfoData/single_site_annotation)

Provides full annotation for list of sites in a single base resolution.

The annotation includes: 

* General annotation: Ensembl gene ID; biotype; gene symbol; HID; Ensembl trenscript ID
* Position in the transcript: exon/ intron ;  5UTR/ 3UTR/ CDS;  position of the site within the transcript relative to TSS
* Translation information (for siteses within CDS): coding frame of the site; codon sequence; amino acid name
* Metagene plots of all input sites 

![pic2](https://user-images.githubusercontent.com/93220699/183313469-d1b6086c-27c0-41ba-ba84-b2b26ffc9a65.png)

**Language: Python3**

**Tools: bedtools**

**Moduls: pybedtools, pandas, numpy, biopython, matplotlib**


