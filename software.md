---
layout: page
title: Software
---

[LongHap](https://github.com/AkeyLab/LongHap): A read-based phasing tool for PacBio HiFi and Oxford Nanopore data that jointly phases SNVs, INDELs, and structural variants and can integrate the 5mC methylation signal already present in long reads.

- Phases more INDELs and SVs than existing read-based tools at lower error rates
- Optional methylation integration extends phase blocks (mean N50 584 kb vs. 443 kb on 38x HiFi HG002)
- Works with HiFi and ONT data
- Roughly 30× faster than MethPhaser

{% include image.html file="/assets/img/longhap.png" align="none" margin-left="5px" margin-right="5px" max-width="800px" alt="LongHap" caption="" credit="Pfennig & Akey, <i>bioRxiv</i>, 2026%}

[MgCod](https://github.com/gatech-genemark/Mgcod): Gene prediction for prokaryotic and phage genomes with stop codon reassignment. MgCod detects which genetic code a genome, or a segment of it, uses and applies the correct model automatically, including in crAssphage genomes that use multiple genetic codes.

{% include image.html file="/assets/img/mgcod.jpg" align="none" margin-left="5px" margin-right="5px" max-width="800px" alt="Mgcod" caption="" credit="Pfennig et al., <i>J Mol Biol</i>, 2023" %}
