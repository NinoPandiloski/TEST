# Co-localization of HP1 isoforms and H3K9me3 in neural stem cells using NGS 

A streamlined pipeline created for the analysis of Cut&Run data. H3K9me3 and HP1 isoform signals are processed using Snakemake to inspect their abundancy, co-localization, and potential redundancy. The files containing the results of the analysis are then processed in R to extract further information.

## Getting Strated

### Program Description

The program takes FastQ files and processes them using Snakemake and R. The following analysis is performed:

* Quality Control (FastQC and MultiQC)
* Mapping (Bowtie2)
* Browsing of the Genome (UCSC)
* Peak calling, Filtering and Annotation (SEACR and bedIntersect)
* Peak analysis and co-localization

### Installing

The Snakefile along with all scripts and configuration files are ready for download 

## Built With

### Snakemake (v. 5.2.4)

* FastQC (v. 0.11.8)
* MultiQC (v. 1.2)
* Bowtie (v. 2.3.4.2)
* Samtools (v 1.9)
* bamCoverage (v. __)
* SEACR (v. 1.3)
* SEACR_R (v. 1.3) 
* BEDTools (v. 2.26.0)
* DeepTools (v. 2.5.4)
  
### R (v. 4.0.0)
* Data parsing and visualization script

## Usage

To use the Snakefile script with all of its configurations on a cluster, use the following code
```
snakemake -j 13 --cluster-config /projects/fs1/nino/bin/config_files/lunarc_config.json --cluster "sbatch -A {cluster.account} -p {cluster.partition} --tasks-per-node {cluster.tasks-per-node}  -t {cluster.time} -o {cluster.o} -e {cluster.e} -J {cluster.J} -N {cluster.N}" --latency-wait 60
```
To use the dry run option and proof check Snakemake's functionality add the flag -n:
```
snakemake -j 13 -n
```

## Acknowledgments


