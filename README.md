Description:
===
This document provides the codes analyzing all the cycling transcriptomes in the article.

Requirements:
===
R 4.0.3

Packages needed to be installed: 

MetaCycle,pheatmap,VennDiagram,ggplot2,cowplot,ggplotify,dplyr,forcats

Usage:
===
Cycling gene identification: 
---
All other species except yeast:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=20,maxper=28, cycMethod = c(“ARS”, “JTK”, “LS”))

For Yeast (high glucose condition):

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=4,maxper=14, cycMethod = c(“ARS”, “JTK”, “LS”),ARSdefaultPer=120,ARSmle=“nomle”)

For Yeast (low glucose condition):

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=5,maxper=15, cycMethod = c(“ARS”, “JTK”, “LS”),ARSdefaultPer=360,ARSmle=“nomle”)

 
Data contained in this paper:
---
All cycling mRNA expression data can be found in the ' All_meta2d_result' folder.

All data about energy cost are located in the 'Energy cost' folder.

Raw input data for gene ontology analysis and enrichment results can be found in 'GO_pather_result'.

Data and codes used in the simulation are in the 'Simulation' folder.

Code in this paper:
---
All codes can be found in the 'Code and plot' folder, and .Rmd files contain the codes for each figure.
