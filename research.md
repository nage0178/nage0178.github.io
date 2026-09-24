---
layout: page
title: Research
---

My research focuses on the intersection of population genetics and phylogenetics, often on questions related to time.
The timing of events is critical to understanding evolutionary history and biological diversity.
For example, these include questions such as whether the extinction of the dinosaurs led to the diversification
of mammals and whether lockdowns decreased the spread of pathogens.
However, estimating the time of biological events is often very difficult. 
I develop novel Bayesian inference methods to infer ages and times, including the timing of a variety of events in multiple systems, including species divergence times using ancient DNA (aDNA), mutation ages in humans, and latency times in HIV using clinical sequence data.
More recently, I have been working on a broader variety of methods and topics, including deep learning and biogeography.


# Inferring ages under the multispecies coalescent 

### Divergence times with ancient DNA 
The multispecies coalescent (MSC) bridges the gap between species trees and gene trees and can be used as a model to infer species tree divergence times. 
I developed a novel method to use tip-dating and the MSC to infer time calibrated phylogenies with aDNA, implemented in the program bpp. 
Alternative methods either do not directly estimate species divergence times or cannot estimate time calibrated tree using information from realistic sample ages. 
Both essential for estimating a species phylogeny with node ages in years. 
I demonstrated that a common approach, given the lack of preexisting methods, biases estimates. 
My analysis of an elephant and woolly mammoth dataset gave strong evidence of aDNA damage, suggesting the need for caution and more complex models when using tip-dating with aDNA.

<ul>
	<li> {% include citation.html
		authors = "<b>Nagel A. A.</b>, Flouri T., Yang Z., & Rannala B."
		title   = "Bayesian Inference Under the Multispecies Coalescent with Ancient DNA Sequences"
		journal = "Systematic Biology"
		biorxiv = "false"
		doi     = "https://doi.org/10.1093/sysbio/syae047"
		year    = "2024"
        youtube = "https://www.youtube.com/watch?v=N-Fwg2DTS8o"
	%} </li>
</ul>

<!-- https://animal-adna.org/blog/2026/04/20/Interview-February-Speaker1/ -->

### Mutation ages and populations of origin

Migration and population structure drive the distribution of polymorphism within and among populations. 
Specific variants are often of interest due to their phenotypic effects, such as disease susceptibility, and their variation among populations, such as skin pigmentation in humans. 
I developed a Bayesian method, MutAnce, which estimates the time and population of origin of SNPs in a structured population with ongoing migration using stochastic mapping. 
The method also estimates the ancestral mutation and the probability of recurrent mutations. 
Both simulations and the analysis of SNPs implicated in human skin pigmentation suggest that both the time and population of origin are difficult to estimate in many cases, likely because the data contain limited information about these variables, while the ancestral state is relatively easy to estimate. 
I also found that several SNPs associated with skin pigmentation may be quite old, arising in the common ancestor of European and Asian populations or the common ancestor of Eurasian and African populations.

<ul>
	<li> {% include citation.html
		authors = "<b>Nagel A. A.</b> & Rannala B."
		title   = "Mutation ages and population origins inferred from genomes in structured populations"
		journal = "Genetics"
		biorxiv = "false"
		doi     = "https://doi.org/10.1093/genetics/iyaf204"
		year    = "2026"
	%} </li>
</ul>


# Timing of HIV latency

HIV currently lacks a cure due to a reservoir of latently infected host cells, which carry HIV proviruses in a reversible state of transcriptional inactivity and are not impacted by treatment.
Reactivation of latent proviruses in the absence of treatment leads to disease progression. 
As such, researchers are interested in understanding the timing of establishment and subsequent reseeding of the latent reservoir. 
I developed a Bayesian phylogenetic tip-dating method, HIVtree, to estimate latent integration times in calendar time using sequence data from individual proviruses and actively replicating viruses within a patient. 
This method is based on the lower mutation rate of latent lineages and was developed from MCMCtree.
I also developed a within-host simulation method.
My method performed well in comparison to existing alternatives, giving accurate and interpretable credible intervals and with lower error, which other methods lacked.
My empirical analysis of clinical samples suggested that many proviruses were integrated around the time of treatment initiation. 

<ul>
	<li> {% include citation.html
		authors = "<b>Nagel A. A.</b> & Rannala B."
		title   = "Bayesian phylogenetic inference of HIV latent lineage ages using serial sequences"
		journal = "Journal of the Royal Society Interface"
		biorxiv = "false"
		doi     = "https://doi.org/10.1098/rsif.2023.0022"
		year    = "2023"
	%} </li>
</ul>

# Deep Learning

Ancestral state reconstruction is a classic problem in phylogenetics. 
It seeks to infer the ancestral state of a character, often for the most recent common ancestors of species (internal nodes). 
Ancestral states are used to investigate ecological and evolutionary hypotheses, such as whether a change in character traits contributed to adaptive radiations or whether traits experienced convergent evolution. 
Existing methods allow for ancestral state reconstruction when there is a tractable likelihood function. 
However, many models that increase biological realism do not have tractable likelihood functions. 
I developed a method to estimate ancestral states with arbitrary models using deep learning. 
I demonstrated that the method performs comparable to Bayesian inference for small trees (50 tips or fewer) for a variety of models, with performance degrading with larger trees. 
Lastly, I applied the method to infer ancestral sequence locations of Ebola from the 2014 West African Ebola virus outbreak using both sample locations and prevalence as input data.

<ul>
    <li> {% include citation.html
        authors = "<b>Nagel A. A.</b> & Landis M. J."
        title   = "Ancestral state reconstruction with discrete characters using deep learning"
        journal = "accepted with major revisions at Systematic Biology"
        biorxiv = "true"
        doi     = "https://doi.org/10.64898/2026.03.19.712918"
        year    = "2026"
    %} </li>
</ul>


# Biogeography with the Multispecies Coalescent 
A longstanding question in biogeography is whether particular speciation events were driven by vicariance or by dispersal. 
Traditionally, this question has either been approached using phylogenetic comparative methods with many species on deep timescales or population genetic methods with very few species on very shallow timescales. 
Using simple simulations as a proof of concept, I suggest that in some cases it may be possible to recover signatures of vicariance and dispersal using gene trees on much deeper timescales than those traditionally studied in phylogeography. 
In particular, gene trees are most likely to be informative about biogeographic histories when studying speciation events preceded (forward in time) by short branches on the species tree relative to the effective population size. 

<ul>
    <li> {% include citation.html
        authors = "<b>Nagel A. A.</b>, Landis M. J., &  Mendes F. K. "
        title   = "Gene tree patterns help answer: vicariance or dispersal?"
        journal = "bioRxiv"
        biorxiv = "true"
        doi     = "https://www.biorxiv.org/content/10.64898/2026.09.17.752061v1"
        year    = "2026"
    %} </li>
</ul>

A link to a talk on my aDNA and HIV work is available [here](https://www.youtube.com/watch?v=iIKR0DXIqcw).
For my most up to date work, see my [Google Scholar](https://scholar.google.com/citations?user=aNr_hhUAAAAJ&hl=en).
