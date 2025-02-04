---
layout: page
title: Research
---

My research focuses on understanding the evolutionary dynamics and implications of admixture and introgression, that is, the mixing of populations that have been separated for relative short and long evolutionary time, respectively. Given their central role to human evolution, I am interested how they have shaped present-day genetic variation and disease risk. To do so, I am integrating population genetics and comparative genomics with bioinformatics tool development. My current research areas include:

**1) Improving de novo genome assembly by integrating methylation information and variant correlations**

Current de novo genome assemblers, like verkko and hifiasm, rely on multiple expensive sequencing experiments, such as parental short-read sequencing or chromosomal contact sequencing, in addition to high-fidelity long-read sequencing (e.g., PacBio Revio sequencing) to generate fully phased genomes. These requirements prohibit the routine de novo assembly of phased genomes at population scale due to the inability to recruit parents for all samples, large amounts of DNA required for each sample, and financial constraints. I am working to improve the phasing in assemblies generated from just high-fidelity long-read data by integrating methylation information and variant correlations from a reference panel. To this end, I have developed a novel read-based phasing algorithm - HiFiHap - specifically for high-fidelity long reads that integrates read methylation information and variant correlations in a reference panel (such as the 1000 Genomes Project) with information from overlapping heterozygous variants between long reads. HiFiHap demonstrates that using methylation information and variant correlations in reference panels significantly improves long-range phasing, achieving a lower error rate and longer contiguously phased blocks (phase block N50) than existing read-based phasing methods (Figure 1). 

