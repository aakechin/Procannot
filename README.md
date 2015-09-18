# Procannot

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
