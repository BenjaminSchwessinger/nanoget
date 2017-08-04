# nanoget
This module provides functions to extract useful metrics from Oxford Nanopore sequencing reads and alignments.  

## FUNCTIONS
Data can be presented in the following formats, using the following functions:  
- A sorted bam file `processBam(bamfile, threads)`  
- A standard fastq file `processFastqPlain(fastqfile)`  
- A fastq file with metadata from MinKNOW or Albacore `processFastq_rich(fastqfile)`  
- A sequencing_summary file generated by Albacore `processSummary(sequencing_summary.txt)`  

Fastq files can be compressed using gzip, bzip2 or bgzip. The data is returned as a pandas DataFrame with standardized headernames for convenient extraction. The functions perform logging while being called and extracting data.


## INSTALLATION
```bash
pip install nanoget
```
or  
[![install with conda](https://anaconda.org/bioconda/nanoget/badges/installer/conda.svg)](https://anaconda.org/bioconda/nanoget)
```
conda install -c bioconda nanoget
```

## STATUS
[![Build Status](https://travis-ci.org/wdecoster/nanoget.svg?branch=master)](https://travis-ci.org/wdecoster/nanoget)
