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

```
