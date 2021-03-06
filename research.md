---
layout: page
title: "Research"
permalink: /research/
main_nav: true
---

### Overview

For biodiversity to arise and accumulate, two processes must occur. First, lineages must split into two or more descendants (i.e. they must speciate), and second, descendant lineages must establish overlapping ranges. 

While the first requirement is obvious, the second follows from the fact that speciation is largely an allopatric process, and allopatry is often achieved when a species’ range is split into two or more isolated subdivisions (i.e. “vicariance”). But vicariance alone is ultimately limited in its ability to generate diversity, as ranges can only be split so many times and still support viable populations. For diversification to continue, lineages must expand geographically to attain range sizes that can bear further subdivision. In nature, this means lineages must often overlap with close relatives. 

Speciation and the establishment of sympatry are thus two critical rate-limiting steps in the diversification cycle. The primary focus of my work is to better understand their most general drivers. 

---
---

<h2 style="text-align:center;"> Questions </h2>

### 1. The role of adaptive ecological divergence in speciation & sympatry

For the past twenty years, evolutionary ecologists have largely viewed diversification through the lens of the ecological theory of adaptive radiation (ETAR; Schluter 2000), an intuitive and influential synthesis in which both speciation and the establishment of sympatry are driven by divergent natural selection. In the theory's classic formulation, reproductive isolation evolves as a consequence of behavioural, phenotypic, or intrinsic genetic changes that accumulate when allopatric lineages adapt in different directions along niche axes such as habitat or diet (“ecological speciation”). Later, when lineages begin to overlap geographically, competition for resources leads to renewed divergent selection and greater ecological divergence (“ecological character displacement”).

Evidence for the ETAR's main tenets has been reported in a number of detailed studies, many of which focus on systems from insular island-like habitats. But these habitats are somewhat specialized, as they often contain fewer species and lower phylogenetic diversity compared to similar-sized areas on continents. Newly discovered patterns of genetic and phenotypic divergence in continental taxa, meanwhile, contradict some expectations of the ETAR. For instance, genomic evidence from tropical avian contact zones show that reproductive isolation readily evolves to virtual completion between lineages with marked ecological similarity (e.g. Pulido-Santacruz et al. 2020, Cronenberger et al. 2020). And a growing number of macroevolutionary analyses conclude that clade-wide diversification is more limited by geographic than ecological opportunity (i.e. opportunity for prolonged allopatry appears to be more important to speciation than opportunity for ecological divergence; e.g. Maestri et al. 2016, Alencar et al. 2017). 

An outstanding question is thus whether ecological divergence is generally required for speciation or coexistence in the more complex ecological theatres commonly found on continents.

Refs.<br>
Schluter, D. 2000. *The Ecology of Adaptive Radiation*, Oxford Univ. Press.<br>
Cronemberger et al. (2020). Evolution. 74: 2512-2525<br>
Pulido-Santacruz, et al. (2020). Evolution. 74: 842-846.<br>
Alencar, et al. (2017). Proc. R. Soc. B., 284: 20171775. <br>
Maestri, et al. (2016). Evolution, 71: 610–632.<br>


#### Approaches

Addressing the generality of adaptive ecological divergence as an engine of diversification requires a comparative statistical approach. While fine-grained ecological details can't feasibly be obtained for very large numbers of lineages, ecological *differences* between closely related species can be inferred from differences in ecomorphology. Such ecological trait measurements are readily obtainable from field and museum specimens. For much of my thesis work, I use and formulate statistical models of trait divergence in sets of closely related lineage pairs. 

**Modelling Divergent Adaptation**: Trait differences between lineages can evolve for a variety of reasons, and indeed differences in trait means will inevitably arise given enough time. A key aim of my work has been to distinguish the statistical signature of trait differences resulting from *divergent selection* -- the driving force behind ecological speciation and character displacement -- versus those that evolve under alternative processes like drift, parallel selection, and fluctuating selection [(**Anderson and Weir, 2020**)](https://doi.org/10.1086/710338).

<img src="/assets/aw2020_fig1.jpg" alt="aw2020fig1" style="width:350px;"/>

**Divergent Adpatation and Speciaton**: One way to infer the generality of ecological speciation is to estimate the proportion of speciating and recently speciated lineages pairs that show evidence of ecology-based divergent selection (ecological speciation's driver). This proportion can be estimated from mixture models in which different pairs in a lineage-pair dataset conform to different underlying processes of functional trait divergence. I've recently described and tested such mixture models (Anderson et al. *Under Review*), several of which are available in the R package [***diverge*** **(version 2.0 and greater)**](https://cran.r-project.org/web/packages/diverge/index.html). 

<img src="/assets/mix_models.jpg" alt="mixmodel" style="width:500px;"/>

**Divergent Adaptation and Sympatry**: Sympatric lineage pairs are often more differentiated in ecomorphology than allopatric pairs, a pattern expected from character displacement. But this pattern can also be produced if lineages are more likely to establish overlapping ranges in the first place if they evolved greater trait differences prior to secondary contact (i.e. 'species sorting'). I recently developed simulation-based models to distinguish these alternatives and found that character displacement better accounts for observed patterns of bill shape differences in pairs of New World terrestrial birds [(**Anderson and Weir 2021**)](https://doi.org/10.1073/pnas.2021209118). 

<img src="/assets/pnas_fig1.jpg" alt="aw2021pnasfig1" style="width:500px;"/>

An additional note on the character displacement models of this paper: previous comparative analyses of character displacement often tested for differences in evolutionary rate between symaptric and allopatric pairs, but an implicit assumption of this approach is that sympatric pairs were always sympatric (even though speciation is agreed to largely require a period of allopatry). A key advance of our character displacement model is that it tests for a shift in selective regime that occurred when lineages are estimated to have become sympatric. 
<br>

---

### 2. Geographic variation in the processes promoting speciation and coexistence

Geographic variation in species richness implies geographic variation in the dynamics of speciation, the establishment of sympatry, colonization, and/or extinction. I'm interested in whether and how the mechanism of speciation and the dynamics of secondary sympatry vary across environments. Ultimately I am interested in how the answer to these questions might help explain broadscale diversity patterns. 

#### Approaches

To test for variation in the dynamics of lineage pair divergence, we can extend trait divergence models to allow key parameters to vary across continuous or categorical variables (e.g. latitude, see [(**Anderson and Weir 2021**)](https://doi.org/10.1073/pnas.2021209118)). A variety of such extended models are available in the *diverge* R package. <br>

<img src="/assets/gradientfig.jpg" alt="gradientfig" style="width:350px;"/>

---

### 3. Reinforcement and the role of sexual interference in preventing the establishment of sympatry

Sympatric close relatives are expected to exhibit sex-related differences that reduce the rate of costly hybridization and other forms of reproductive interference. A growing body of recent work has suggested that 'good' biological species are often prevented from establishing sympatry due to a lack of such pre-mating isolation, as the production of unfit hybrids in contact zones renders those areas demographic sinks (Mikkelsen and Irwin 2021, Irwin and Schluter 2021). In some cases, especially in Amazonian birds, these contact zones can persist for hundreds of thousands and even millions of years (e.g. Pulido-Santacruz et al. 2020). One possibile explanation is that selection for reinforcement (i.e. evolution of premating barriers as an adaptive response to reproductive interference) in the contact zone is swamped out by gene flow from from other areas in a lineages' range <span>&#8212;</span> areas in which hybridization does not occur and thus individuals are not subject to reinforcing selection. 

I'm interested in the dynamics of reinforcement and in the apparent *inability* of some lineages to evolve premating isolation for long periods. A key question is what demographic or evolutionary changes are required to destabilize this stable range limit <span>&#8212;</span> what needs to occur in order for postzygotically isolated lineages to finally evolve premating barriers and broadly overlap? 