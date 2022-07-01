# captcr-snakemake
Author: Arnavaz.Danesh@uhnresearch.ca
Orginal repo: https://github.com/arnavaz/cap-tcr

This repository is to automate the pughlab captcr pipeline using a snakemake workflow
The pipeline consists of barcode extraction, running mixcr, running QC, and clonetracking


# Intallation requirements
1. Python
2. Biopython (python package)
3. pandas (python package)
4. numpy (python package)
5. matplotlib (python package)
2. R
3. ggplot2 (R-package)
4. ggalluvial  (R-package)
5. randomcoloR   (R-package)



# Run with example data

```shell
# clone the repo
salloc -c 1 -t 2:00:00 --mem=6G -p build

git clone https://github.com/LupienLab/cap-tcr.git

# Update config file
vi config.yaml

# Run Snakemake or submit a job
snakemake -S Snakefile --cores 1

```
