# [Completing Circular Bacterial Genomes With Assembly Complexity by Using a Sampling Strategy From a Single MinION Run With Barcoding](https://www.frontiersin.org/articles/10.3389/fmicb.2019.02068/full)

## Background

During this residential training, you will acquire skills in high throughput sequence analysis, the use of reproducible genomic workflows and download data using APIs. Through this mini-project, you will get to solidify and consolidate the skills you will have acquired. 

## Abstract
The Oxford Nanopore MinION is an affordable and portable DNA sequencer that can produce very long reads (tens of kilobase pairs), which enable de novo bacterial genome assembly. Although many algorithms and tools have been developed for base calling, read mapping, de novo assembly, and polishing, an automated pipeline is not available for one-stop analysis for circular bacterial genome reconstruction. In this paper, we present the pipeline CCBGpipe for completing circular bacterial genomes. Raw current signals are demultiplexed and base called to generate sequencing data. Sequencing reads are de novo assembled several times by using a sampling strategy to produce circular contigs that have a sequence in common between their start and end. The circular contigs are polished by using raw signals and sequencing reads; then, duplicated sequences are removed to form a linear representation of circular sequences. The circularized contigs are finally rearranged to start at the start position of dnaA/repA or a replication origin based on the GC skew. CCBGpipe implemented in Python is available at https://github.com/jade-nhri/CCBGpipe. Using sequencing data produced from a single MinION run, we obtained 48 circular sequences, comprising 12 chromosomes and 36 plasmids of 12 bacteria, including Acinetobacter nosocomialis, Acinetobacter pittii, and Staphylococcus aureus. With adequate quantities of sequencing reads (80×), CCBGpipe can provide a complete and automated assembly of circular bacterial genomes.


## Your Task
1. Download the sequence data programmatically using an API
2. The project uses CCBGpipe implemented in Python is available and packaged in Docker for reproducibility. The first task is to reproduce the analysis as is by following the documentation provided in the README 
3. Reproduce the analysis workflow used for genome assembly of Oxford Nanopore MinION using Nextflow or Snakemake, and Singularity for containerization


## Questions
In your report, you should address the following question:
- Are you able to arrive at similar conclusions as those in the paper? Why or why not? 
- What else can you glean from your re-analysis?
- Are the descriptions in the methodology section detailed for reproducibility? If not, what could you have done to improve reproducibility?
