---
layout: page
title: "Research"
permalink: /research/
main_nav: true
---

For species richness to evolve in a clade, two processes must occur. First, lineages must split into two or more descendants (i.e. they must speciate), and second, descendant lineages must establish overlapping ranges. 

While the first requirement is self-evident, the second follows from the fact that speciation is largely an allopatric process, and allopatry is often achieved when a species’ range is split into two or more isolated subdivisions (i.e. “vicariance”). **But vicariance alone is ultimately limited in its ability to generate diversity**, as ranges can only be split so many times and still support viable populations. For diversification to continue, lineages must expand geographically to attain range sizes that can bear further subdivision. In nature, this means lineages must often overlap with close relatives. 

Speciation and the establishment of sympatry are thus two critical rate-limiting steps in the diversification cycle. The primary focus of my research is to better understand their drivers. 

---

<h2 style="text-align:center;"> Questions </h2>

### 1. The role of ecological divergence in speciation and the establishment of sympatry

For the past twenty years, evolutionary ecologists have largely viewed diversification through the lens of the ecological theory of adaptive radiation (ETAR; Schluter 2000), an intuitive and influential synthesis in which both speciation and the establishment of sympatry are driven by divergent natural selection. In the theory's classic formulation, reproductive isolation evolves as a consequence of behavioural, phenotypic, or intrinsic genetic changes that accumulate when allopatric lineages adapt in different directions along niche axes such as habitat or diet (“ecological speciation”). Later, when lineages begin to overlap geographically, competition for resources leads to renewed divergent selection and greater ecological divergence (“ecological character displacement”).

Evidence for the ETAR's main tenets has been reported in a number of detailed studies, leading many authors to suggest that adaptive radiation is a generally important mechanism in diversification. However, many of these studies have focused on systems from insular island-like habitats. Newly discovered patterns of genetic and phenotypic divergence in continental taxa, meanwhile, contradict some expectations of this framework. For instance, genomic evidence from tropical avian contact zones show that reproductive isolation readily evolves to virtual completion between lineages with marked ecological similarity. And a growing number of macroevolutionary analyses conclude that clade-wide diversification is more limited by geographic than ecological opportunity. 

An outstanding question is whether ecological divergence is generally required for speciation or coexistence in the complex ecological theatres in which diversity most generally evolves.

Schluter, D. 2000. *The Ecology of Adaptive Radiation*, Oxford Univ. Press.

#### Approaches

Addressing the generality of ecological divergence as an engine of diversification requires a comparative statistical approach. While fine-grained ecological details can't feasibly be obtained for very large numbers of lineages, ecological *differences* between closely related species can be inferred from differences in ecomorphology. Such ecological trait measurements are readily obtainable from field and museum specimens. I thus work with and formulate statistical models and simulation-based models of trait divergence between closely related lineage pairs. 

**Modelling Divergent Adaptation**: Trait differences between lineages can arise for a variety of reasons, and indeed evolved differences in trait means are inevitable given enough time. A key aim of my work has been to distinguish the statistical signature of trait divergence resulting from *divergent selection* -- the driving force behind ecological speciation and character displacement -- versus alternative processes like drift, parallel selection, and fluctuating selection (Anderson and Weir, 2020).

**Addressing Speciaton**: One way to infer the generality of ecological speciation is to estimate the proportion of speciating and recently speciated lineages pairs that show evidence of ecology-based divergent selection (ecological speciaiton's driver). This proportion can be estimated from mixture models in which different pairs in a lineage-pair dataset conform to different underlying processes of functional trait divergence. I've recently described and tested such mixture models (Anderson et al. *Under Review*), several of which are available in the R package *diverge* (version 2.0 and greater). 

**Addressing Sympatry**: Sympatric lineage pairs are often more differentiated in ecomorphology than allopatric pairs, a pattern expected from character displacement. But this pattern can also be produced if lineages are more likely to establish overlapping ranges in the first place if they evolved greater trait differences prior to secondary contact (i.e. 'species sorting'). I recently developed simulation-based models to distinguish these alternatives and found that character displacement better accounts for observed patterns of bill shape differences in New World terrestrial birds (Anderson and Weir 2021). 

Previous comparative analyses of character displacement often tested for differences in evolutionary rate between symaptric and allopatric pairs, but an implicit e assumption of this approach is that sympatric pairs were always sympatric (speciation is agreed to largely require a period of allopatry). A key advance of our character displacement model is that it tests for a shift in selective regime when lineages are estimated to have become sympatric. 


### 2. Geographic variation in the processes promoting speciation and coexistence

Geographic variation in species richness implies geographic variation in speciation, the establishment of sympatry, colonization, and/or extinction. I'm interested in whether and how the mechanism of speciation and the dynamics of secondary sympatry vary across environments. Ultimately I am interested in how the answer to these questions might help explain broadscale diversity patterns. 

#### Approaches

To test for variation in the dynamics of lineage pair divergence, we can extend trait divergence models to allow key parameters to vary across continuous or categorical variables (e.g. latitude, pollinator type). A variety of such extended models are available in the *diverge* R package. 

{% comment %} 

### 3. Reinforcement and the role of sexual interference in preventing the establishment of sympatry

Ecological competition has long been considered an important factor determining when and if species coexist, but interactions related to sex may also have important and overlooked consequences for range overlap. Such 'sexual interference' includes the production of maladapted hybrids as well as less-well-understood interactions like (factoften-overloooked factor is that of sexual interference between closely related lineages. 'Sexual interference' refers to costly interactions related to sex (rather than ecological resource use).


{% endcomment %} 