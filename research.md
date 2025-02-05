---
layout: page
title: Research
---

My research focuses on understanding the evolutionary dynamics and implications of admixture and introgression, that is, the mixing of populations that have been separated for relatively short and long evolutionary time, respectively. Given their central role in human evolution, I am interested in how they have shaped present-day genetic variation and disease risk. To do so, I am integrating population genetics and comparative genomics with bioinformatics tool development. My current research areas include:

### Improving de novo genome assembly by integrating methylation information and variant correlations

{% include image.html
    src="assets/img/hifihap.png" <!-- image filename (placed in /assets/images) -->
    alt="Figure 1" <!-- alt text -->
    description="This is Jekyll's logo, featuring Dr. Jekyll's serum!" <!-- Caption -->
%}

<p><img src="assets/img/hifihap.png"
    width="500" 
    alt="Figure 1" align="right">
</p>
<p>
  <em>**Figure 1.** Benchmarking of HiFiHap and state-of-the-art read-based phasing tools (i.e., HaploMaker, Whatshap, HapCUT2, and WhatsHap + MethPhaser) using PacBio Revio HiFi 40x data for HG002 from the HPRC and the HG002 T2T Q100 ground truth call set for small variants. For HiFiHap, 1000 Genomes Project phase 3 data was additionally used for population-based phasing. For each tool, we assessed the switch error rate (A) and phase block N50 (B) using WhatsHap. Note that HaploMaker does not provide phase block information. Each dot represents a chromosome.</em>
</p>
Current de novo genome assemblers, like verkko and hifiasm, rely on multiple expensive sequencing experiments, such as parental short-read sequencing or chromosomal contact sequencing, in addition to high-fidelity long-read sequencing (e.g., PacBio Revio sequencing) to generate fully phased genomes. These requirements prohibit the routine de novo assembly of phased genomes at population scale due to the inability to recruit parents for all samples, large amounts of DNA required for each sample, and financial constraints.  I am working to improve the phasing in assemblies generated from just high-fidelity long-read data by integrating methylation information and variant correlations from a reference panel. To this end, I have developed a novel read-based phasing algorithm - HiFiHap - specifically for high-fidelity long reads that integrates read methylation information and variant correlations in a reference panel (such as the 1000 Genomes Project) with information from overlapping heterozygous variants between long reads. HiFiHap demonstrates that using methylation information and variant correlations in reference panels significantly improves long-range phasing, achieving a lower error rate and longer contiguously phased blocks (phase block N50) than existing read-based phasing methods (Figure 1). 

| ![Figure 1](assets/img/hifihap.png). |
|:--:| 
| **Figure 1.** Benchmarking of HiFiHap and state-of-the-art read-based phasing tools (i.e., HaploMaker, Whatshap, HapCUT2, and WhatsHap + MethPhaser) using PacBio Revio HiFi 40x data for HG002 from the HPRC and the HG002 T2T Q100 ground truth call set for small variants. For HiFiHap, 1000 Genomes Project phase 3 data was additionally used for population-based phasing. For each tool, we assessed the switch error rate (A) and phase block N50 (B) using WhatsHap. Note that HaploMaker does not provide phase block information. Each dot represents a chromosome.|

### Developing a tool suite for population and statistical genetics analyses on pangenomes

Pangenomes are a set of multiple whole-genome sequences typically represented as a graph (Figure 2). Unlike a single reference genome, pangenomes capture the full spectrum of genetic variation by being able to represent multiple mutations at the same position and accommodate substantial amounts of non-reference sequence. These capabilities are particularly critical for studying biomedically important highly diverse and structurally complex “genomic black holes” that are now accurately reconstructed in de novo genome assemblies. However, due to an absence of analytical tools to analyze pangenomes, current approaches map genetic variation in pangenomes back to the coordinate system of a single reference genome and analyze it with conventional methods, which largely defeats the advantages of de novo assembly. Thus, the absence of analytical tools for pangenomes prevents us from taking advantage of the full spectrum of genetic variation (in particular, structurally complex variation) in population and statistical genetics analyses. To address this, I am currently developing a tool suite to support standard population and statistical genetics analyses (e.g., elucidating population structure, association testing, etc.) on pangenomes.

| ![Figure 2](assets/img/pangenomes.jpg). |
|:--:| 
| **Figure 2.** An illustration of the advantages of a pangenome graph over a single linear reference genome (Source, [NHGRI](https://www.genome.gov/sites/default/files/inline-images/Pangenome-tube-map.jpg)).|

### Theoretical and empirical population genetics of admixture and introgression
Admixture and introgression play a central role in human evolution. Therefore, it is critical to understand how these processes have shaped the distribution of present-day genetic variation and what its implications are. I introduced a novel population genetics model that accounts for a heterogeneous genetic background in hybrid genomes, showing that fitness effects arising from a heterogeneous background modify the dynamics of focal alleles during introgression. The model predicts that most introgressed alleles must survive an initial filter, suggesting Neanderthal-introgressed variants in extant human genomes cannot be that harmful. I empirically tested this hypothesis using 30,780 predominantly African- and European-like admixed genomes from the United States. In such genomes, the fitness of Neanderthal introgressed variants was re-evaluated as most Neanderthal introgressed sequence was contributed by European-like ancestors and brought onto a “novel” African-like genetic background (Figure 3). In concordance with predictions of my theoretical model, I found that remaining Neanderthal ancestry in contemporary genomes is likely evolutionary neutral as the admixed genomes contained approximately as much Neanderthal introgressed sequence as expected, suggesting widespread recent polygenic selection did not occur. Furthermore, in related work, I proposed methods for including uncertainty in the interpretation of sex-biased admixture in the Americas in the context of the transatlantic slave trade. I collaborated on studies elucidating the genetic basis of prostate cancer and male pattern baldness in African men.
| ![Figure 2](assets/img/neanderthal.jpg). |
|:--:| 
| **Figure 3.** Secondary contact has brought Neanderthal DNA into novel genomic contexts. (1) Neanderthal DNA introgressed into non-African populations ~50 kya, leading to an initial purging of Neanderthal ancestry. (2) During the past 15 generations, recent admixture of individuals with African-like ancestry and European-like ancestry has introduced Neanderthal variants into a novel genetic background, potentially leading to secondary selection. |
