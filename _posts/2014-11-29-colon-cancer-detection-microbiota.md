---
layout: post
title: Using gut microbiota to detect colon cancer
permalink: 2014-11-29-colon-cancer-detection-microbiota.html
date: 2014-11-29 12:03:00
categories: [Article]
tags: [colon, cancer, metagenomics, microbiota]
fullview: false
---


A study[^1] published in [Molecular System Biology](http://bit.ly/crcmicrob) showed how gut microbiota could be used to detect colon cancer in combination with standard fecal occult blood test ([FOBT](http://en.wikipedia.org/wiki/Fecal_occult_blood)). The potential is huge as the detection could be increased notably for early stage cancer (where curation have a better prognostic notably).

<a href="http://bit.ly/crcmicrob"><img itemprop="image" src="http://d3dwu2jylmmhzr.cloudfront.net/sites/default/files/highwire/msb/10/11/766/embed/graphic-1.gif" alt="crc msb snapshot"/></a>

As a co-authors, I would like to give some additional insight regarding this paper like a "making of", we could say. First of all, this study is the consequence of a fruitful collaboration between important institution between France (AP-HP) and Germany (EMBL, DKFZ). The most challenging part was to get samples in a right way directly from hospital, to improve current machine learning method to adapt them to metagenomics data and to devellop protocol to study the tumor environment. {{more}} <!--more-->

### Getting samples ###

<img itemprop="image" src="http://hopital-necker.aphp.fr/wp-content/blogs.dir/14/files/2012/06/logo-aphp.jpg" alt="AP-HP" style="float: left; border: 20px solid white; width: 150px;"/>
Getting samples from patient in real life is complex and it is difficult to follow high gold standard from microbial ecologist recommandations. This part was done in the gastoenterology departement at Henri Mondor hospital (France). The main difficulty was to take stool sample in a right way before the coloscopy which is the gold standard to confirm the presence of cancer. The inclusion took two years between 2004 and 2006 before the [take off of gut metagenomics](http://julientap.com/post/2011-04-19-metagenomics-text-mining.html) and notably the first gut metagenomics papers published by Gill, Pop et al in 2006[^2].


### Improving bioinformatics tools ###

<img itemprop="image" src="http://bioinfo-fr.net/wp-content/uploads/2013/07/logo_embl.jpg" alt="EMBL" style="float: left; border: 20px solid white; width: 150px;"/>
Big consortia such as MetaHIT and HMP made possible to improve bionformatics tools and give a comprehensive view of the gut microbiota notably by making gut genes catalog[^3], discovering of enterotypes[^4], releasing of numerous gut bacterial genomes[^5] and having a better delineation of microbial species[^6]. In addition with this study, we developped a dedicated pipeline to build classification models in order to detect colon cancer patient according their gut metagenomes. Althought those machine learning methods are well known already, one of the biggest enemy of such large data analysis is the "overfitting": having the impression to find biomarkers just by chance, unstable and with no relation with a biological signal. To test our model made with this pipeline, we included a larger external and independent  validation cohort including samples from DKFZ and [my.microbes](http://my.microbes.eu/) study. 

### Focusing on tumor microbiome ###

<img itemprop="image" src="http://www.dkfz.de/microscopy2008/dkfz.jpg" alt="DKFZ" style="float: left; border: 20px solid white; width: 150px;"/> 
Another technical challenge was to explore the tumor environment itself to bring new indication about mechanism of cancer progression. This was done at DKFZ improving existing protocol and using one of last sequencing technology in order to track microbial biomarkers from stool to the tumor itself.

### Emphasing new perspectives ###

Standard FOBT is well know to have a low sensitivity (colon cancer detection rate ~50%) but combining it with metagenomics allow to go over 70% keeping an high specificity. Furthermore, some bacterial species used in the model are even enriched when we focussed on the tumor microbiome. Whole metagenomics allow to dig gene content of the colon cancer microbiome and we observed a metabolic shift from fiber degradation in controls to utilization of host carbohydrates and amino acids in colon cancer patients, accompanied by an increase of lipopolysaccharide metabolism.

Those findings open new perspectives in colon cancer medical care management. New detection test could be developped and getting gene content from screened patients could lead also to some prevention through diet for example.


----------


### References ###
[^1]: Zeller G, Tap J, Voigt AY et al. [Potential of fecal microbiota for early‐stage detection of colorectal cancer](http://bit.ly/crcmicrob). 2014. Molecular Systems Biology 10:766

[^2]: Gill, Pop et al. [Metagenomic analysis of the human distal gut microbiome.](http://www.sciencemag.org/content/312/5778/1355.long) Science. 2006 Jun 2;312(5778):1355-9.

[^3]: J Qin et al. MetaHIT consortium. [A human gut microbial gene catalogue established by metagenomic sequencing](http://www.nature.com/nature/journal/v464/n7285/abs/nature08821.html). 2010. Nature 464 (7285), 59-65

[^4]: M Arumugam, J Raes et al. MetaHIT consortium. [Enterotypes of the human gut microbiome](http://www.nature.com/nature/journal/v473/n7346/abs/nature09944.html). 2011. Nature 473 (7346), 174-180

[^5]: Nelson KE et al. [A catalog of reference genomes from the human microbiome](http://www.ncbi.nlm.nih.gov/pubmed/20489017). Science 2010 May 21

[^6]: Mende et al. [Accurate and universal delineation of prokaryotic species](http://www.nature.com/nmeth/journal/v10/n9/abs/nmeth.2575.html). Nature methods 10 (9), 881-884