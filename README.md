# c3ds-2026

This repository holds my scripts and notes from the UCSF C3 Data Science
Bootcamp, where I learn R, git & machine learning.

## Week 2 day 1

- CoreHPC interface in Open OnDemand
- Format for asking for support 
- Running Rscript at the command line

## Tools
- **R studio**
- Positron
- [Open OnDemand](https://chpc-ucsf-ondemand-vm1.corehpc.ucsf.edu/)

## Examples
```sh
sbatch --job-name=dti_$tnum \
--mem=32G --cpus-per-task=32 \
--time=02:00:00 \
 -o processing_logs/dti_${serial}.log \
 -e processing_logs/dti_${serial}.log \
 --wrap="process_DTI_brain_RT ${Enum}/${serial} $tnum"
```

