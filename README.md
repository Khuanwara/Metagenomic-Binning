# Metagenomic-Binning
The Bowmodel is a multi-stage binning method designed to enhance metagenomic analysis. It proceeds through the following stages: (1) assembling reads into contigs, (2) extracting compositional features, (3) computing contig similarity, (4) structuring complex networks, and (5) clustering. This study primarily focuses on the contig similarity computation stage, a critical component of the binning process. Contigs are initially grouped based on their length ranges. Similarity between contigs is then calculated using a combination of compositional similarity and coverage difference. This hybrid similarity metric, when integrated with the Louvain clustering algorithm, demonstrates strong performance in terms of the number of bins identified.

# Installation
1. First clone the BowModel repository to a local directory. Note that BowModel only supports linux.

git clone https://github.com/yourname/binning_project.git
cd binning_project
pip install .

2. Then run following command to run the tool.
   `binning-run [CONTIG_FASTA] [Composition Features_TSV] --out [OUT_DIR]`
   Some basic Git commands are:
```
git status
git add
git commit
```
# Required File Formats
Contig File
Contig file from metaSPAdes tool containing the genomes in following format.

Composition Features File
Composition Features File from iLearn tool 
