# Pipeline-RNASeq-DESeq2
Automated RNA-Seq analysis pipeline using DESeq2 and GEO data

This repository contains a fully automated, reproducible R/Bioconductor pipeline for bulk RNA-Seq differential expression analysis using `DESeq2`. 

## 🚀 Features
* **Automated Data Retrieval:** Uses `GEOquery` to automatically download supplementary raw count matrices directly from the NCBI Gene Expression Omnibus (e.g., GSE254974).
* **Dynamic Metadata Parsing:** Automatically detects categorical experimental variables from GEO metadata to build the `DESeqDataSet`, avoiding hardcoded group names and ensuring reusability across different studies.
* **Publication-Ready Visualizations:** Includes customized, high-aesthetics Volcano Plots (`ggplot2`) and Heatmaps (`pheatmap`) tailored for scientific reporting.

## 📊 Visualizations

### Gene Expression Heatmap
*Displays the top 30 most significant differentially expressed genes across samples, maintaining biological clustering while optimizing aesthetics.*
![Heatmap]([HeatmapGSE254974.png](https://github.com/alcafuz34/Pipeline-RNASeq-DESeq2/blob/main/GraphicsGSE254974/HeatmapGSE254974.png)

### Volcano Plot
*Highlights significantly up- and down-regulated genes across the entire transcriptome (padj < 0.05, |Log2FC| > 1), with dynamic axis scaling.*
![Volcano Plot][(VolcanoPlot.png)](https://github.com/alcafuz34/Pipeline-RNASeq-DESeq2/blob/main/GraphicsGSE254974/VolcanoPlot.png)

## 🛠️ Usage
1. Clone this repository to your local machine.
2. Open the `.Rmd` file in RStudio.
3. Click **Knit** to automatically download the dataset, run the complete DESeq2 pipeline, and generate the final HTML/PDF report.

## 👨‍🔬 Author
**Julissa Vargas Alcafuz**  
Biochemist | Diploma in Bioinformatics and Computational Biology, Universidad de Chile.
