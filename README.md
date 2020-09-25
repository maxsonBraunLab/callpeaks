![TestCallpeaks](https://github.com/maxsonBraunLab/callpeaks/workflows/TestCallpeaks/badge.svg?branch=master)

# callpeaks

Custom peak caller for CUT&amp;TAG data relies heavily on the [Regulatory Genomics Toolbox](https://github.com/CostaLab/reg-gen) API. 

## Setup

Clone this repository, or download the file `wget https://raw.githubusercontent.com/maxsonBraunLab/callpeaks/master/callpeaks.py`. Then set up dependencies using conda.

```
# create a conda environment from the environment file
cd callpeaks
conda env create -f callpeaks-env.yml
conda activate callpeaks-env

python callpeaks.py -h
usage: callpeaks.py [-h] -b BAM -o OUTFILE [-cf CONTROLFILE] -cs CHROMSIZES
                    [-minreads MINREADS] [-minsize MINSIZE] [-pv PVALUE]
                    [-cp CORRECT_PVAL]

Call peaks on CUTTAG bam files

optional arguments:
  -h, --help            show this help message and exit
  -b BAM, --bam BAM     Bam file
  -o OUTFILE, --outfile OUTFILE
                        Output prefix (filename without extension)
  -cf CONTROLFILE, --controlfile CONTROLFILE
                        control file for experiment or sample
  -cs CHROMSIZES, --chromsizes CHROMSIZES
                        Genome chromsizes file
  -minreads MINREADS, --minreads MINREADS
                        Minimum number of reads
  -minsize MINSIZE, --minsize MINSIZE
                        Only output peaks greater than or equal to -min-size
  -pv PVALUE, --pvalue PVALUE
                        Pvalue threshold for binomial peak test (default 0.05)
  -cp CORRECT_PVAL, --correct-pval CORRECT_PVAL
                        Correct p-values for multiple testing using
                        Benjamini/Hochberg ("bh") or Benjamini/Yekutieli
                        ("by") method
```
