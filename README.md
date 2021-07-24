Description:
===
This document provides the analysis code for all the data and images mentioned in this article

Requirements:
===
R 4.0.3

Packages needed to be installed: MetaCycle,pheatmap,VennDiagram,ggplot2,cowplot,ggplotify,dplyr,forcats

Usage:
===
Cycling gene calculation: 
---
All species expect yeast:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=20,maxper=28, cycMethod = c(“ARS”, “JTK”, “LS”))

Yeast high glucose:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=4,maxper=14, cycMethod = c(“ARS”, “JTK”, “LS”),ARSdefaultPer=120,ARSmle=“nomle”)

Yeast low glucose:

meta2d(infile=input_file, filestyle=“csv”, outdir=output_file,timepoints=“Line1”,outRawData=TRUE,minper=5,maxper=15, cycMethod = c(“ARS”, “JTK”, “LS”),ARSdefaultPer=360,ARSmle=“nomle”)

 
Data contained in this paper:
---
All mRNA level expression data in this paper can be found at' All_meta2d_result' folder.

All data about calculating energy cost can be found at 'Energy cost' folder.

Gene ontology raw input data and enrich result can be found at 'GO_pather_result' folder.

Data that simulation required can ben found at 'SImulation' folder.

Code in this paper:
---
All code in this paper can be found in 'Code and plot' folder, and all .md files contains figures in this paper.
