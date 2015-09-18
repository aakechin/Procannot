# procannot

Procannot annotates SNPs in procaryotic genomes

## Getting started

git clone https://github.com/aakechin/procannot.git

## Introduction

Procannot is a software package for annotating SNPs from bacteria genomes. It consists of several algorithms of annotation: by genes' information, its presense in our SNP database, influence on organism's pathways and evolution selection type of all genes. All of algorithms uses our databases that can be updated or created by user. Generally Procannot consists of the following databases:
* GenBank_files - contains all GenBank files of all organisms;
* GenomeDB - contains files with information about all genes;
* GenomeSeq - contains files with nucleotide sequences of all genomes;
* Organisms - contains information about all organisms that were written to the databases;
* PathwayDB - contains information about all pathways of all strains;
* SnpDB - contains all SNPs that were found between all strains of an organism;
* OrthoDB and alignedOrthoDB - contain alignments of genes of all strains of an organism.

## Availability

Procannot is released under GPLv3. The latest source code is freely available at github. After you acquire the source code, install python version 3 or higher and then use it. You can install Python3 with the following command:

sudo apt-get install python3

## Manual

All commands and their options you can find by use of -h option or in the Manual.pdf file.

## Examples of use

All commnads of procannot must be run from the installation directory.

To create all databases that were listed above for Bacillus subtilis (reference NC_000964), run the command:

```python3 procannot.py make_all -o 'Bacillus subtilis' -r NC_000964```

To create only database of genes' information run the command:

```python3 procannot.py make_genomedb -o 'Bacillus subtilis'```

If you already have database of genes for this organism and want to create database with orthologues for this reference of an organism, run the command:

```python3 procannot.py make_orthodb -o 'Bacillus subtilis' -r NC_000964```


