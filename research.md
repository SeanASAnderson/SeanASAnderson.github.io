---
layout: page
title: "Research"
permalink: /research/
main_nav: true
---

### Overview

I study the ecology and evolution of non-model organisms in order to draw inferences about how biodiversity tends to evolve. My ultimate aim is to better understand the mechanisms that generate observable patterns of species richness. 

My work is grounded in a basic premise, which is that for biodiversity to arise and accumulate, two processes must occur. First, lineages must split into two or more descendants (i.e. they must (a) speciate and (b) resist sliding back into a hybrid swarm), and second, descendant lineages must establish overlapping ranges. 

While the first requirement is obvious, the second follows from the fact that speciation is largely an allopatric process, and allopatry is often achieved when a species’ range is split into two or more isolated subdivisions (i.e. “vicariance”). But vicariance alone is ultimately limited in its ability to generate diversity, as ranges can only be split so many times and still support viable populations. For diversification to continue, lineages must expand geographically to attain range sizes that can bear further subdivision. In nature, this often that means lineages must overlap with close relatives. 

Speciation and the establishment of sympatry are thus two critical rate-limiting steps in the diversification cycle. The primary focus of my work is to better understand the factors affecting these processes. 

<!--Finally, while nature is certainly idiosyncratic, it is ultimately necessary to generalize when attempting to explain broader-scale patterns of diversity. For this reason, a major focus of my work is data synthesis and the use of statistical models to draw general inferences about the mechanisms driving (or halting) progress toward the origin of new species...and how variation in these factors can help explain the unequal distribution of global biodiversity-->

---
---

<h2 style="text-align:center;"> Questions </h2>

### 1. The role of adaptive ecological divergence in speciation & sympatry

The idea that speciation is partly an ecological process dates to Darwin and Wallace at the very beginning of modern evolutionary thought <span>&#8212;</span> but the concept remains a central area of contemporary speciation research within the sub-field of evolutionary ecology. Indeed, for the past twenty-plus years, evolutionary ecology's leading framework for diversification has been the ecological theory of adaptive radiation (ETAR; [Schluter 2000](https://global.oup.com/academic/product/the-ecology-of-adaptive-radiation-9780198505228?cc=us&lang=en&)), a powerful synthesis which holds that two key phases of speciation (allopatric divergence and the establishment of sympatry) are both driven by ecology-based divergent natural selection. In the theory's classic formulation, reproductive isolation begins to evolve as a consequence of behavioural, phenotypic, or intrinsic genetic changes that accumulate when allopatric lineages adapt in different directions along niche axes such as habitat or diet (“ecological speciation”). Later, when lineages begin to overlap geographically, competition for resources leads to renewed divergent selection and greater ecological divergence (“ecological character displacement”). 

Strong evidence for the ETAR's main tenets has been reported in a number of meticulous studies, many of which focus on very young taxa that reside in insular habitats such as lakes and oceanic islands. Such habitats tend to contain fewer species (and thus fewer predators and competitors) than similar-sized areas on continents, and in this respect they provide exceptionally favourable conditions for rapid and pronounced adaptive evolution (i.e. "ecological release", [Herrmann et al. 2020](https://doi.org/10.1016/j.tree.2020.10.019); and "ecological opportunity" [Stroud and Losos 2016](https://doi.org/10.1146/annurev-ecolsys-121415-032254)). 

One major focus of my research is to build upon this pioneering work and to assess general support for ecological divergence as a driver of speciation under a wider range of ecological conditions. For example, it is likely that continental lineages seldom experience circumstances as amenable to adaptive ecological divergence as do taxa on islands -- and yet continental lineages diversify nonetheless. Given that most described species have arisen in this continental context, a critical question is to what extent adaptive ecological divergence is generally required for speciation or coexistence when lineages evolve in these more complex ecological theatres.

#### Approaches

Addressing the generality of adaptive ecological divergence as an engine of diversification requires a comparative statistical approach. While fine-grained ecological details can't feasibly be obtained for very large numbers of lineages, ecological *differences* between closely related species can be inferred from differences in their ecomorphology. Such ecological trait measurements are readily obtainable for numerous organisms both in the field and from museum specimens. My PhD work involved formulating statistical models of trait divergence in sets of closely related lineage pairs and deploying these models to analyze organismal data. 

**Modelling Divergent Adaptation**: Trait differences between lineages can evolve for a variety of reasons, and indeed differences in trait means will inevitably arise given enough time. A focus of my PhD work was to develop statistical models of trait differentiation that distinguish the signature of *divergent selection* -- the driving force behind ecological speciation and character displacement -- from alternative processes like drift, parallel selection, and fluctuating selection [(**Anderson and Weir 2020, *Am. Nat.***)](https://doi.org/10.1086/710338). These models and several of their extensions are in my R package [***diverge***](https://cran.r-project.org/web/packages/diverge/index.html).

<img src="/assets/aw2020_fig1.jpg" alt="aw2020fig1" style="width:350px;"/>

**Divergent Adaptation and Allopatric Speciaton**: A paradox of speciation research is that most speciation events are thought to require a period of allopatric evolution, but speciation ecology is typically studied in sympatric taxa. There is a good reason for this scenario; namely, reproductive isolation is best studied where it is tested in nature. But it raises the question of to what extent adaptive ecological divergence occurs during the all-important allopatric phase of speciation <span>&#8212;</span> a phase to which researchers have paid relatively little attention. Even within adaptive radiation theory, the role of adaptive ecological divergence in speciation's allopatric phase is an open question ([Losos 2009 p.291-292](https://www.ucpress.edu/book/9780520269842/lizards-in-an-evolutionary-tree), [Rundell and Price 2009](https://doi.org/10.1016/j.tree.2009.02.007), [Price 2010](https://doi.org/10.1098/rstb.2009.0269))

I recently addressed this problem as it pertains to several groups of birds, mammals, and amphibians [**(Anderson and Weir 2022, *Science*)**](https://doi.org/10.1126/science.abo7719). In this paper, we describe new mixture models in which different pairs in a lineage-pair dataset conform to different underlying processes of ecological trait divergence (e.g. divergent v. parallel adaptation or parallel adaptation v. phenotypic drift). The models allow us to estimate the proportion of allopatric pairs in a given dataset whose trait differences correspond to theoretical expectations of these alternative underlying processes. 

We found that regardless the trait or dataset in question, relatively few pairs in any particular analysis (out of 130 analyses) are best described by a divergent adaptation model. Instead, an overwhelming proportion of pairs are better described by models of parallel adaptive evolution. It thus appears that allopatric speciation is most generally characterized by lineages adaptively evolving under similar rather than divergent ecology-based selective pressures. Ecological divergence may yet be important later in speciation as lineages begin to overlap geographically. 

The mixture models are now available in the R package [***diverge*** **(version 2.0 and greater)**](https://cran.r-project.org/web/packages/diverge/index.html).

<img src="/assets/aw2022_fig3.jpg" alt="fig3histogram" style="width:500px;"/>

**Divergent Adaptation and Sympatry**: Sympatric lineage pairs are often more differentiated in ecomorphology than allopatric pairs. This pattern is the expected outcome from character displacement <span>&#8212;</span> but this pattern can also be produced if lineages that evolve greater differences in allopatry are more likely to establish overlapping ranges upon secondary contact (i.e. 'species sorting'). I recently developed simulation-based models to distinguish these alternatives and found that character displacement better accounts for observed patterns of bill shape differences in a continental group of allopatric and sympatric pairs of New World terrestrial birds [(**Anderson and Weir 2021, *PNAS***)](https://doi.org/10.1073/pnas.2021209118).

<img src="/assets/pnas_fig1.jpg" alt="aw2021pnasfig1" style="width:500px;"/>

An additional note on the character displacement models of this paper: previous comparative analyses of character displacement often tested for differences in evolutionary rate between sympatric and allopatric pairs, but an implicit assumption of this approach is that sympatric pairs were always sympatric (even though speciation is agreed to largely require a period of allopatry). A key advance of our character displacement model is that it tests for a shift in selective regime that occurred when lineages are estimated to have become sympatric. 
<br>

---

### 2. Factors affecting speciation reversal

The road to origin of species is not a one-way street. While barriers to gene flow can quickly arise between lineages under some circumstances, such barriers can also quickly dissolve when circumstances change, resulting in incipient species collapse. In fact, growing evidence supporting an ephemeral speciation model ([Rosenblum et al. 2012](https://link.springer.com/article/10.1007/s11692-012-9171-x)) suggests that incipient species readily arise but are generally short-lived, and it seems likely that extinction-via-hybridization or 'speciation reversal' is a major reason. This observation points to a major consequence: to cultivate a mechanistic understanding of the build-up of biodiversity, researchers will require a much better grasp of how stable, non-ephemeral reproductive barriers tend to evolve in nature. 

In a new perspective paper, I call attention this problem and synthesize available evidence with respect to the unknown role of ecological adaptation in the evolution of unconditional or 'intrinsic' reproductive isolation [(**Anderson et al. 2023, *Am. Nat.***)](https://doi.org/10.1086/723763).

I have also launched a new research project with Daniel Matute into the evolution of intrinsic isolation between two species of wild *Drosophila* (*D. santomea and D. yakuba)*. These species form a natural hybrid zone (one of the only known for *Drosophila* in the wild) on the island of S&atilde;o Tom&eacute;, which straddles the equator off the coast of west Africa. There, the two species displace one another across an ecological gradient on the slopes of Pico de S&atilde;o Tom&eacute;, the island's highest peak, with *D. yakuba* occurring at lower elevations and the endemic *D. santomea* occupying the higher slopes. This system touches on the two major themes of my research <span>&#8212;</span> speciation and the factors affecting coexistence.

**I recently completed a field expedition in which I sampled the first-ever elevational transect on the northwest slope of the mountain**. I am currently using the resulting genomic data to test alternative hypotheses regarding irreversible barriers to introgression and their ecological basis. I am also formulating analytical and simulation-based models to generate intuition regarding the build-up of intrinsic isolation in these and other taxa. 

---

### 3. Geographic variation in the processes promoting speciation and coexistence

Geographic variation in species richness implies geographic variation in (a) the dynamics of speciation, the (b) establishment of sympatry, (c) colonization, and (d) extinction -- or a combination of these factors. I'm interested in whether and how the mechanism of speciation and the dynamics of secondary sympatry vary across environments.

#### Approaches

To test for variation in the dynamics of lineage pair divergence, we can extend trait divergence models to allow key parameters to vary across continuous or categorical variables (e.g. latitude, [(**Anderson and Weir 2021, PNAS**](https://doi.org/10.1073/pnas.2021209118) and [**(Anderson and Weir 2022 Science)**](https://doi.org/10.1126/science.abo7719). A variety of such extended models are available in the *diverge* R package. I have recently begunt to expand this approach to test for geographic variation in the strength of different forms of reproductive isolation in numerous taxa. <br>
<img src="/assets/gradientfig.jpg" alt="gradientfig" style="width:350px;"/>

---

### 4. Reinforcement and the role of sexual interference in preventing the establishment of sympatry

Sympatric close relatives are expected to exhibit sex-related differences that reduce the rate of costly hybridization and other forms of reproductive interference. A growing body of recent work has suggested that 'good' biological species are often prevented from establishing sympatry due to a lack of such pre-mating isolation, as the production of unfit hybrids in contact zones renders those areas demographic sinks ([Mikkelsen and Irwin 2021](https://onlinelibrary.wiley.com/doi/abs/10.1111/mec.16015), [Irwin and Schluter 2021](https://www.journals.uchicago.edu/doi/abs/10.1086/720365)). In some cases, especially in Amazonian birds, these contact zones can persist for hundreds of thousands and even millions of years (e.g. [Pulido-Santacruz et al. 2020](https://onlinelibrary.wiley.com/doi/abs/10.1111/evo.13902)). One possible explanation is that selection for reinforcement (i.e. evolution of premating barriers as an adaptive response to reproductive interference) in the contact zone is swamped out by gene flow from other areas in a lineages' range <span>&#8212;</span> areas in which hybridization does not occur and thus individuals are not subject to reinforcing selection. 

I'm interested in the dynamics of reinforcement and in the apparent *inability* of some lineages to evolve premating isolation for long periods. A key question is what demographic or evolutionary changes are required to destabilize this stable range limit <span>&#8212;</span> what needs to occur in order for postzygotically isolated lineages to finally evolve premating barriers and broadly overlap? 
