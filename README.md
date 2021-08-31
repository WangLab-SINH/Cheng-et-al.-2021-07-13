Description:
===
This document provides the analysis codes for all the data and figures mentioned in the article

Requirements:
===
R 4.0.3

Packages needed to be installed: MetaCycle,pheatmap,VennDiagram,ggplot2,cowplot,ggplotify,dplyr,forcats

Usage:
===
Cycling gene calculation: 
---
All species except yeast:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=20,maxper=28, cycMethod = c(“ARS”, “JTK”, “LS”))

Yeast high glucose:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=4,maxper=14, cycMethod = c(“ARS”, “JTK”, “LS”),ARSdefaultPer=120,ARSmle=“nomle”)

Yeast low glucose:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=5,maxper=15, cycMethod = c(“ARS”, “JTK”, “LS”),ARSdefaultPer=360,ARSmle=“nomle”)

 
Data contained in this paper:
---
All mRNA expression data in this paper can be found in the ' All_meta2d_result' folder.

All data about energy cost can be found in the 'Energy cost' folder.

Raw input data for gene ontology analysis and enrichment result can be found in  'GO_pather_result'.

Data and codes used in the simulation are in the 'Simulation' folder.

Code in this paper:
---
All codes can be found in the 'Code and plot' folder, and all .Rmd files contain the codes for each figures.
