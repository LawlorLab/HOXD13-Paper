# HOXD13-Paper

Processed data and downstream analysis of scRNA Seq experiments for the paper HOXD13 is a direct EWS-FLI1 target and moderates fusion-dependent transcriptional states. This repository includes the R script that will replicate panels from Figure 7 the paper. To process the data you can pull in the matrix files from GEO and run the code. 

Attached files:

1. HOXD13_Paper_data_Analysis.Rmd This R markdown file should allow for complete analysis of the data and reproduction of the figures from the paper. To start you will need to go to the GEO page (GSE) and download the 2 tar.gz files and put them into your wd. Then using the code you should be able to pull them in and run the code.

2. Genesets needed for the analysis as .txt files to pull in.
    -ICEWS_genes_78.txt. :list from Aynaud et al. 2020 of their highly specific EWS-FLI1 signature genes
    -HOXD13_EF_genesets.txt: text file that has both the EF and HOXD13 activated genes in one file. 
    -HOXD13_activated.txt: Significant HOXD13 activated genes in both CHLA10 and A673 cells
    -HOXD13_repressed.txt: Significant HOXD13 repressed genes in both CHLA10 and A673 cells
    -kinsey_EF_activated.txt: list from Kinsey et al. 2016 of EWS-FLI1 activated genes in EWS502 and TC71 cells. 
    -kinsey_EF_represseded.txt: list from Kinsey et al. 2016 of EWS-FLI1 repressed genes in EWS502 and TC71 cells. 
    -mesenchyme_dev.txt: list from GO:0060485 mesenchyme development gene set. 


3. Data for the public PDX samples (Aynaud et al. 2020). 
-Go here and download the text files that I used in my code to just pull in and made the CDS object https://xfer.curie.fr/get/4kbMMiYPx8K/Ewing_sarcoma_scRNASeq.zip (if this does not work go through the github.com/sysbio-curie/EwingSingleCellDataAnalysis

**the cell ranger data for these files also is at: Series GSE130024 (https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE130024)
