# RNA-seq
RNA-seq code with Bowtie alignment and generating strain-specific counts using Emase

Publication from our lab "https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6404261/" Chris Baker had determined QTL locations using the BxD mouse panel, that impact recombination hotspot activation in germ cells. These QTLs impact many loci in cis and in trans in the mouse genome. 
The Macfarlan group (https://elifesciences.org/articles/56337#content) had knocked out these QTL regions in germ cells and we were interested to know if these regions impact expression of QTL targets or not. If yes, this would be the functional validation of the QTLs and how they impact hotspot activation. 
As part of my initial learning of computational genomics, I analyzed RNA-seq data of the chr4-QTL region KO in germ cells obtained from the Macfarlan group. 

First, I performed QC and trimmed off the adaptors from the RNA-seq data. Then, I aligned the reads using Bowtie2 and obtained the counts using EMASE (https://emase.readthedocs.io/en/latest/). Once I obtained the counts, I analyzed the data further in R. 

Final Results: We did not obtain a lot of peak overlaps between the two datasets (QTL and RNA expression) but the overlaps that we found were found to be significant (as determined by the Fishers exact test). 
