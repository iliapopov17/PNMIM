### Abstract

This study investigates gut microbiota variations in children aged 36-45 months, examining the impact of different facilities. Utilizing amplicon sequencing and advanced statistical analyses, significant microbial differences, notably in wastewater disposal and toilets, were revealed. These findings illuminate potential factors influencing early gut microbiota composition, offering insights for targeted interventions to enhance children's gut health.

### Materials and Methods

- _Data Collection:_
Stool samples from children participating in the study underwent amplicon sequencing (`FASTQ`) for microbiota analysis.

- _Data Processing:_
`Qiime2` and `DADA2` were employed for the denoising process, ensuring high-quality data for subsequent analysis.

- _Taxonomic Identification:_
`Silva NGS` was utilized to assign taxonomic labels to the denoised sequences, enhancing the precision of microbial identification.

- _Statistical Analysis:_
Rarefaction, normalization, and filtering steps to minimize false positives and transform `ASV` counts into taxa relative abundance was made in `RStudio`.

- _Association Analysis:_
The `MaAsLin2` and `LinDA` packages were instrumental in constructing linear models to elucidate associations between gut microbiota profiles and various parameters such as nutritional status, anthropometric measurements, and hygiene practices.

- _Visualization:_
Custom visualizations using `ggplot2` facilitated a clear and insightful representation of the associations uncovered by the linear models.

<div style='justify-content: center'>
<img src="https://github.com/iliapopov17/PNMIM/blob/main/imgs/metagenomic_pipeline.png" align='center', width="100%">
</div>

_Figure 1. Pipeline overview._

### Results

The results are presented as a heatmap (Figure 1), where each element represents the logarithm of the binary ratio (log2fc) of the abundance of different microbial taxa in different types of facilities (e.g. wastewater disposal systems, clean water sources, industrial premises and toilets).

Positive log2fc values (displayed in green) indicate an increase in abundance, while negative values (purple) indicate a decrease. Each row represents a specific microbial taxon and each column corresponds to the type of object. The darker the colour, the more pronounced the changes.

Significant variations are highlighted, especially in sewage disposal systems and toilets, indicating potential microbiota features in these locations. This graphical approach enriches our understanding of the influence of different facilities on microbiota composition and identifies potential factors influencing changes in the microbial ecosystem.

 ### Discussion

The observed variations in microbial abundance, particularly in wastewater disposal systems and toilets, suggest the potential impact of specific facilities on the gut microbiota of children. These findings underscore the need for further exploration of environmental factors influencing early microbial colonization, providing valuable insights for targeted interventions to promote optimal gut health in this critical age group.

### Data availability

In this repository you can find:

1) [`PNMIM-report.Rmd`](https://github.com/iliapopov17/PNMIM/blob/main/02_Metagenomic_assay/PNMIM-report.Rmd) - contains a script to process the raw data and run [`MaAsLin2`](https://github.com/biobakery/Maaslin2)
2) [`PNMIM-report.html`](https://github.com/iliapopov17/PNMIM/blob/main/02_Metagenomic_assay/PNMIM-report.html) - contains the report on the study in `.html` format
3) [`Sanitation_Genus_rel_abund/figures/heatmap.png`](https://github.com/iliapopov17/PNMIM/blob/main/02_Metagenomic_assay/Sanitation_Genus_rel_abund/figures/heatmap.png) - contains standart heatmap pictured by [`MaAsLin2`](https://github.com/biobakery/Maaslin2)
4) [`Heatmaps/genus_sanitation.png`](https://github.com/iliapopov17/PNMIM/blob/main/02_Metagenomic_assay/Heatmaps/genus_sanitation.png) - contains exactly the same heatmap, but more beautiful and in publication ready quality

### Publication

Results are published in:

[Surono, I.S., Popov, I., Verbruggen, S., Verhoeven, J., Kusumo, P.D., Venema, K. Gut microbiota differences in stunted and normal-length children aged 36–45 months in East Nusa Tenggara, Indonesia. PLoS ONE 19, e0299349 (2024).](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0299349) https://doi.org/10.1371/journal.pone.0299349

### Data Availability

Raw sequences and metadata have been deposited in the [Sequence Read Archive under Bioproject number PRJNA1065733](https://dataview.ncbi.nlm.nih.gov/object/PRJNA1065733).<br>
All data are available as of Jan 17, 2024.
