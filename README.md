# singularity_tsd_dna

## Overview
This is the definition file used to generate tapestri dna on-prem v.1.15 pipeline

## Build
use singularity build to create a .sif container image

## Required input
/host_path/input: A folder contains conf.yaml, Read1.fq.gz and Read2.fq.gz
/host_path/output: A folder that you have write access to. (make sure the selinux context is set correctly)

## Usage
singularity run -B /host_path/input:/data/input -B /host_path/output:/data/output /path/to/dna_pipeline.sif 
