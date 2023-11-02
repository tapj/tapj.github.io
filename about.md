---
layout: page
title: About
permalink: about.html
---



<!--<div itemscope itemtype="http://schema.org/Person">

I am <a href="http://julientap.com" itemprop="url"> <span itemprop="name">Julien Tap</span></a> and 
I am currently working as <span itemprop="jobTitle">microbial ecologist</span> and data analyst at 
<span itemprop="affiliation">Danone research</span> located in <span itemprop="address" itemscope itemtype="http://schema.org/PostalAddress">
<span itemprop="addressRegion">Ile de France</span>. 
You can also check my <a itemprop="sameAs" href="http://www.linkedin.com/in/julientap" >linkedin profile</a>.

</div>

</div>-->


<div itemscope itemtype="http://schema.org/Person">

Julien is currently <span itemprop="jobTitle">research scientist</span> at <span itemprop="affiliation">INRAE</span> center settled in Paris-Saclay campus where he is working on microbiome science topics around nutrition and human health.

After several internships in microbiology at Institut Pasteur (Patrick Grimont, Philippe Glaser, Sylvain Brisse), <span itemprop="name">Julien Tap</span> went to Joel Doré's Lab to do a PhD headed by Marion Leclerc (Jan 2007 to Dec 2009). His main project was to study dietary fiber impact on human gut microbiota using notably metagenomic and metatranscriptomic approach.

Since his PhD, his research interest focused on interactions between nutrition, gut microbiota and human health. This allowed him to work with different AP-HP clinicians like Pr Karine Clément and Pr Iradj Sobhani. As post-doc both at EMBL in Peer Bork’s group and at INRA Metagenopolis unit (Joel Doré, Dusko Ehrlich), he used approaches like numerical ecology and machine learning technics to untangle big omics data with clinical and dietary data in health and disease. At Danone Research, he contributed to generate novel scientific evidence on fermented products on human gut microbiome more precisely using functional analysis and he studied large-scale data to move to more personalized approaches taken gut microbiome into account. 

</div>

### Research experience

* _Since October 2022_  [INRAE Micalis Institute](https://www.micalis.fr/)  - Jouy-en-Josas - France

* _2015 - 2022_  Danone Nutricia Research  - Palaiseau - France

* _2013 - 2014_ INRA : [Metagenopolis](http://www.mgps.eu) – (D. Ehrlich, J. Doré) - Jouy-en-Josas - France

* _2010 - 2012_ EMBL : [Bork group](http://bork.embl.de) Computational Biology –  (P. Bork)  Deciphering function and evolution of biological systems - Heidelberg - Germany

* _2007 - 2009_ Phylogenetic and Functional Biodiversity of the Human Gut Microbiota - Ecology and Physiology of the Digestive Tract (UEPSD) - INRA - Jouy-en-Josas – (M.Leclerc, J. Doré)

	>_Thesis project_ : Diet impact on structural and functional dynamics of the human intestinal microbiota

* _March/September 2006_ Bacterial population genetics labs - Biodiversity of Emerging Pathogenic Bacteria - Pasteur Institute – (S. Brisse, P. Grimont) Paris XV

	>_Master’s degree project_: genetic structure of _M. prototuberculosis_ and origin of _M. tuberculosis_

* _March/August 2005_ Unit of Genomics of Microbial Pathogens Pasteur Genopole® Île-de-France - Pasteur Institute - (P. Glaser, C. Buchrieser, F. Kuntz) Paris XV

	>_Master’s degree project_ : Development of a biodiversity DNA chips for molecular typing of _Listeria_

* _April/July 2004_ National Reference Center for E. coli - Biodiversity of Emerging Pathogenic Bacteria - Pasteur Institute - (F. Grimont, P. Grimont) Paris XV

	>_Bachelor’s degree project_ : molecular characterization of _E. coli_ O111 and the diversity of isolated strains in France

---------------------------------------------------------

### Education

* _2007-2009_ University of Pierre & Marie Curie Paris VI
        **Ph.D.** in Physiology and Pathophysiology

* _2005-2006_ Pierre & Marie Curie Paris VI
        **Master’s degree** in Molecular Biology and Cellular - Genetics specialty

* _2001-2005_ Paris Val de Marne University Paris XII
	*  **“Maitrise”**. Biotechnology and bio-industry .
	* **Bachelor’s degree.** Biological engineering - Biochemical and Food specialty

-----------------------------------------------

### Publications

for up-to-date bibliography check: 
* my [Google Scholar](http://scholar.google.com/citations?user=aYTQ-WkAAAAJ) profile
* my [PubMed publication list](http://www.ncbi.nlm.nih.gov/pubmed?term=Tap%20Julien[Full%20Author%20Name])
* my [ORCID profile](https://orcid.org/0000-0001-8998-5413)



<table>
  <thead>
    <tr>
      <th>Year</th>
      <th>Title & Details</th>
      <th>Citations</th>
    </tr>
  </thead>
  <tbody>
    {% for publication in site.data.publications_google_scholar %}
    <tr>
      <td>{{ publication.year }}</td>
      <td>
        <strong><a href="{{ publication.pubid }}">{{ publication.title }}</a></strong><br>
        {{ publication.author }}<br>
        <em>{{ publication.journal }}</em><br>
        {{ publication.number }}
      </td>
      <td>{{ publication.cites }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
