# Whole-Genome Sequencing Pipeline
This repository provides scripts and workflows for a whole-genome sequencing (WGS) pipeline, focusing on alignment, variant calling, and structural variant analysis.

# Pipeline Steps
1. Preprocessing
- Quality control with FastQC.
- Alignment using BWA-MEM.

3. Variant Calling and Filtering
- Single nucleotide variant (SNV) calling with GATK.
- Structural variant (SV) detection using MANTA and AnnotSV.

4. Post-processing
- Filtration and annotation with bcftools and SVDB.

5. Requirements
- GATK
- BWA-MEM
- MANTA
- SAMtools, bcftools

# Usage
Run scripts in PBS environment by submitting .pbs files for each step.
