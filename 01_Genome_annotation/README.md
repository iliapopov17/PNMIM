### Abstract

Ensuring the safety of probiotic strains utilized in human and animal trials is imperative. The emergence of genome-based safety assessments for probiotics, marked by their cost-effectiveness and expeditious nature, has become an integral component of national regulations governing probiotic-containing foods in Indonesia. This report delves into the genome-based safety assessment of the probiotic strain _Lpb. plantarum_ IS-10506, employing advanced bioinformatic tools to explore bacteriocin clusters and CRISPR sequences. The study contributes valuable insights for a comprehensive understanding of probiotic safety, aligning with the evolving landscape of regulatory frameworks.

### Materials and methods

The genome of the probiotic strain _L. plantarum_ IS-10506 was sequenced using Nanopore, assembled, annotated and screened for useful genomic features.To predict the bacteriocin clusters and their organization BAGEL4 software was used[^1].
The anticipation of CRISPR (clustered regularly interspaced short palindromic repeats) sequences was accomplished using CRISPRCasFinder[^2].

### Results

#### Bacteriocin Production

Upon scrutinizing the complete genome sequence of _Lpb. plantarum_ IS-10506 isolate, a genetic location associated with the production of bacteriocin (_pln_ locus) was detected. The assessment of this strain demonstrated the presence of genes responsible for the synthesis of two peptides, namely plantaricin _plnF_ (class IIb) and _plnE_ (unclassified) (Figure 1 & Table 1). These peptides were previously identified in other _Lpb. plantarum strains_[^3].

<div style='justify-content: center'>
<img src="https://github.com/iliapopov17/PNMIM/blob/main/imgs/BAGEL_results.jpg" align='center', width="100%">
</div>

_Figure 1. An outline of the plantaricin operons observed in the evaluated Lpb. plantarum IS-10506 is presented. Gene maps exhibit the full plantaricin sections, wherein the arrows represent ORFs that are color-coded based on their projected functions. Additionally, BAGEL4 was used to predict the promotors and terminators, which are also highlighted in the maps._

|_pln_ genes|Function|Amino acid sequence|
|---|---|---|
|plnF|Bacteriocin|MKKFLVLRDRELNAISGGVFHAYSARGVRNNYKSAVGPADWVISAVRGFIHG|
|plnE|Bacteriocin|MLQFEKLQYSRLPQKKLAKISGGFNRGGYNFGKSVRHVVDAIGSVAGIRGILKSIR|

_Table 1. Amino acids sequence of the plantaricin encoding genes belonging to the pln locus._

#### CRISPRCas

_Lpb. plantarum_ IS-10506 is projected to possess a type II CRISPR-Cas system, which includes four cas genes – _cas9_, _cas1_, _cas2_, and _cns2_. The primary attributes of the CRISPR system are summarized in Table 2.
The CRISPR systems that contain clustered regularly interspaced short palindromic repeats could target protospacer sequences stored in the CRISPR array, which provides a defensive mechanism against phages and plasmids that have been previously encountered (Table 3).

|Gene name|Genome position start|End|Orientation|
|---|---|---|---|
|cas9_TypeII|2,193,294|2,197,370|+|
|cas1_TypeII|2,197,565|2,198,470|+|
|cas2_TypeI-II-III|2,198,448|2,198,753|+|
|csn2_TypeIIA|2,198,750|2,199,427|+|

_Table 2. Genomic features of CRISPR-Cas system in Lpb. plantarum IS-10506._

|Feature|Description|
|-------|-----------|
|Start|2199452|
|End|2200081|
|DR consensus|GTCTTGAATAGTAGTCATATCAAACAGGTTTAGAAC|
|DR length|36|
|Spacer count|9|
|Direction|+|

_Table 3. Analysis of CRISPR II system direct repeats._

### Discussion

The genomic exploration of _L. plantarum_ IS-10506 reveals a sophisticated genetic architecture, providing a foundation for its safety assessment. The presence of bacteriocin-encoding genes underscores its antimicrobial potential, crucial for its probiotic functionality. Simultaneously, the identified CRISPR-Cas system suggests a defense mechanism against foreign genetic elements. 


### Publication

Results are published at:

[Umanets, A., Surono, I.S. & Venema, K. I am better than I look: genome based safety assessment of the probiotic Lactiplantibacillus plantarum IS-10506. BMC Genomics 24, 518 (2023).](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-023-09495-y) https://doi.org/10.1186/s12864-023-09495-y

> You can find me in the [`Acknowledgements`](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-023-09495-y#Ack1) section

### References

[^1]:	van Heel, A. J. et al. BAGEL4: a user-friendly web server to thoroughly mine RiPPs and bacteriocins. Nucleic Acids Res 46, W278–W281 (2018).
[^2]:	Couvin, D. et al. CRISPRCasFinder, an update of CRISRFinder, includes a portable version, enhanced performance and integrates search for Cas proteins. Nucleic Acids Res 46, W246–W251 (2018).
[^3]:	da Silva Sabo, S., Vitolo, M., González, J. M. D. & Oliveira, R. P. de S. Overview of Lactobacillus plantarum as a promising bacteriocin producer among lactic acid bacteria. Food Res Int 64, 527–536 (2014).
