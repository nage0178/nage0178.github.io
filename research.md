---
layout: page
title: Research
---

The timing of events is critical to understanding evolutionary history and biological diversity.
For example, questions such as whether the extinction of the dinosaurs lead to the diversification
of mammals and whether climatic change drove genetic adaptation depend critically on the times
of events. Despite the fundamental importance of the time, estimating the time of biological
events is often very difficult. 
My research focuses on the development of novel Bayesian inference methods to infer ages and time.
I estimate times of a variety of types of events in multiple systems, including latency
times using  species divergence times with ancient DNA (aDNA), mutation ages with human data from the 1000 Genomes Project, and within-host viral sequences.
I seek to understand the statistical performance of new and existing methods and the limitations of the data through simulation studies.


# Inferring ages with under the multispecies coalescent 

### Divergence times ancient DNA 
The multispecies coalescent (MSC) bridges the gap between species trees and gene trees can be used as model to infer species tree divergence times. 
I developed a novel method to use tip-dating and the MSC to infer time calibrated phylogenies with aDNA, implemented in the program bpp. 
Alternative methods do not directly estimate species divergence times or cannot estimate time calibrated tree using information for realistic sample ages, both of which are essential to estimating a species phylogeny with node ages in years. 
I demonstrated a common approach given the lack of preexisting methods biases estimates. 
Analysis of an elephant and woolly mammoth dataset gave strong evidence of aDNA damage, suggesting the need for caution and more complex models when using tip-dating with aDNA.

<ul>
	<li> {% include citation.html
		authors = "<b>Nagel A. A.</b>, Flouri T., Yang Z., Rannala B."
		title   = "Bayesian Inference Under the Multispecies Coalescent with Ancient DNA Sequences"
		journal = "Systematic Biology"
		biorxiv = "false"
		doi     = "https://doi.org/10.1093/sysbio/syae047"
		year    = "2024"
	%} </li>
</ul>

### Mutation ages and populations of origin

Migration and population structure drive the distribution of polymorphism within and among populations. 
Specific variants are often of interest due to their phenotypic effect, such as disease susceptibility, and strong variation among populations, such as skin pigmentation in humans. 
I developed a Bayesian method, MutAnce, which estimates the time and population of origin of SNPs in a structure population with ongoing migration using stochastic mapping. 
The method also estimates the ancestral mutation and the probability of recurrent mutation. 
Both simulations and the analysis of SNPs implicated in human skin pigmentation suggest that both the time and population of origin are difficult to estimate in many cases, likely because there is a limited amount of information in the data about these variables, while the ancestral state is relatively easy to estimate. 
While the method may not have much power in some cases, it does accurately reflect the uncertainty in the data in the credible intervals (sets). 

<ul>
	<li> {% include citation.html
		authors = "<b>Nagel A. A.</b> & Rannala B."
		title   = "Mutation ages and population origins inferred from genomes in structured populations"
		journal = "bioRxiv"
		biorxiv = "true"
		doi     = "https://doi.org/10.1101/2025.01.28.635333"
		year    = "2025"
	%} </li>
</ul>

# HIV latency

HIV currently lacks a cure due to a reservoir of latently infected host cells, which carry the HIV provirus in a reversible state of transcriptional inactivity and are not impacted by treatment.
Reactivation of latent proviruses in the absence of treatment leads to disease progression. 
As such, researchers are very interested in understanding the timing of establishment and subsequent reseeding of the latent reservoir. 
I developed a Bayesian phylogenetic tip-dating method, HIVtree, to estimate latent integration times in calendar time using sequence data from individual proviruses and actively replicating viruses within a patient. 
This method is based off the lower mutation rate of latent lineages and was developed from MCMCtree.
I also developed of a within-host simulation method.
My method performed well in comparison to existing alternatives, giving accurate and interpretable credible intervals and with lower error, which other methods lacked.

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

A link to a talk on my aDNA and HIV work is [here](https://www.youtube.com/watch?v=iIKR0DXIqcw).
For my most up to date work, see my [google scholar](https://scholar.google.com/citations?user=aNr_hhUAAAAJ&hl=en).
