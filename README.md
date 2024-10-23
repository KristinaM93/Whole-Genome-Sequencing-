# Whole-Genome-Sequencing-
markdown
Copy code
# Structural Variant Analysis Pipeline

This repository provides a pipeline for structural variant (SV) analysis using a combination of popular bioinformatics tools: **BWA-MEM**, **GATK**, **Manta**, **bcftools**, **AnnotSV**, and **SVDB**. The pipeline allows users to align sequencing data, call structural variants, annotate variants, and analyze results effectively.

## Table of Contents

- [Tools](#tools)
- [Installation](#installation)
- [Usage](#usage)
- [Example Workflow](#example-workflow)
- [Results](#results)
- [Contributing](#contributing)
  
## Tools

1. **BWA-MEM**: A fast and accurate algorithm for mapping low-divergent sequences against a large reference genome.
2. **GATK (Genome Analysis Toolkit)**: A toolkit for variant discovery in high-throughput sequencing data.
3. **Manta**: A tool for detecting structural variants from whole-genome and targeted sequencing data.
4. **bcftools**: A set of utilities for manipulating variant calls in the BCF and VCF formats.
5. **AnnotSV**: A tool for annotating structural variants with various databases and resources.
6. **SVDB**: A database of structural variants for comprehensive analysis.

## Installation

conda install -c bioconda bwa gatk manta bcftools annotsv

## Usage

bash run_pipeline.sh -i <input_fastq_dir> -r <reference_genome> -o <output_dir>

## Parameters 

-i <input_fastq_dir>: Directory containing input FASTQ files.
-r <reference_genome>: Reference genome file (FASTA format).
-o <output_dir>: Directory for output results.

## Example Workflow 

1. Align Reads: Use BWA-MEM to align the reads to the reference genome.
2. Mark Duplicates: Use GATK to mark duplicate reads.
3. Call Variants: Use Manta to call structural variants.
4. Filter Variants: Use BCFtools to filter the variant calls.
5. Annotate Variants: Use AnnotSV to annotate the filtered variants.
6. Store Results: Use SVDB to store and analyze results.

## Results 

The output directory will contain the following files:
1. Aligned BAM files
2. Variant call files (VCF)
3. Annotated variant files


## Contributing

Contributions are welcome! If you have suggestions for improvements or want to add new features, please open an issue or submit a pull request.
