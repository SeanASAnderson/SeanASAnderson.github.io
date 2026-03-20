---
layout: page
title: "Research"
permalink: /research/
main_nav: true
---

<!--### Overview-->

We study the ecology and evolution of non-model organisms to better understand how biodiversity tends to evolve. Our work blends computational biology with field biology and evolutionary ecology with evolutionary genetics, and we address fundamental questions surrounding the mechanisms that generate observable patterns of species richness. 

Conceptually, our work is organized around a basic premise, which is that for biodiversity to arise and accumulate, two processes must occur. First, lineages must split into two or more descendants (however defined), and second, descendant lineages must establish overlapping ranges. Speciation and the establishment of sympatry are then two critical rate-limiting steps in the diversification cycle. The primary focus of our work is to better understand the factors affecting both processes. 

Practically, we work with a variety of organisms and data types. One component of our research involves the fine-grained investigation of genomic and ecological patterns in individual lineages pairs (ranging from wild drosophilids to butterfies to fishes); other questions involve large-scale data syntheses and comparative analyses, which often necessitate the development of novel statistical approaches; and still another component of our work involves the construction of mechanistic theory to generate testable predictions. 

A non-exhaustive list of recent and on-going research themes are:

- The role of adaptive ecological divergence during speciation and the establishment of sympatry
- The role of ecological differences in preventing lineage fusion upon secondary contact
- Factors affecting speciation reversal
- The relationship (or lack thereof) between organismal RI (mechanisms like hybrid sterility or assortative mating) and evolutionary RI (the extent of independent evolution across two genomes) 
- The relationship between evolutionary RI as measured across contemporary hybrids zones and over deeper timescales
- Understanding the speciation continuum from the perspective of both organismal and evolutionary RI

Our current work is framed in the context of a revolution in our understanding of speciation that has emerged in the genomic age and that is not yet near complete. For instance, just prior to the routine publication of whole genomes, Coyne and Orr (2004) exhaustively surveyed the speciation literature and concluded "our guess is that morphologically distinct taxa showing rampant gene exchange at many loci will be rare" (p.41). We now know that such data are commonplace, that strong organismal RI doesn't always translate into reduced gene flow -- and, most radically (in the context of Modern Synthesis thought), that stable co-occurrence between diagnosable taxa does not imply a lack of introgression. Diagnostic trait differences can indeed be maintained despite weak evolutionary RI. 

A key priority in our current age is thus to develop research questions that (1) treat RI as continuous rather than discrete, (2) recognize the reversibility of the proecess, and (3) are, rather paradoxically, agnostic about species status. One question that meets these criteria also forms the unifying question of our current work: ***how and why does the extent of independent evolution across the genomes of two lineages rise or fall over time?***


---
---

<!--

<h2 style="text-align:center;"> Recent Questions We Have Addressed </h2>

### The role of adaptive ecological divergence during speciation & the establishment of sympatry

The idea that speciation is partly an ecological process dates to Darwin and Wallace at the very beginning of modern evolutionary thought <span>&#8212;</span> but the concept remains a central area of contemporary speciation research within the sub-field of evolutionary ecology. For the past twenty-plus years, evolutionary ecology's leading framework for diversification has been the ecological theory of adaptive radiation (ETAR; [Schluter 2000](https://global.oup.com/academic/product/the-ecology-of-adaptive-radiation-9780198505228?cc=us&lang=en&)), a powerful synthesis which holds that two key phases of speciation (allopatric divergence and the establishment of sympatry) are both driven by ecology-based divergent natural selection. In the theory's classic formulation, reproductive isolation begins to evolve as a consequence of behavioural, phenotypic, or intrinsic genetic changes that accumulate when allopatric lineages adapt in different directions along niche axes such as habitat or diet (“ecological speciation”). Later, when lineages begin to overlap geographically, competition for resources leads to renewed divergent selection and greater ecological divergence (“ecological character displacement”). 

Strong evidence for the ETAR's main tenets has been reported in a number of meticulous studies, many of which focus on very young taxa that reside in insular habitats such as lakes and oceanic islands. Such habitats tend to contain fewer species (and thus fewer predators and competitors) than similar-sized areas on continents, and in this respect they provide exceptionally favourable conditions for rapid and pronounced adaptive evolution (i.e. "ecological release", [Herrmann et al. 2020](https://doi.org/10.1016/j.tree.2020.10.019); and "ecological opportunity" [Stroud and Losos 2016](https://doi.org/10.1146/annurev-ecolsys-121415-032254)). 

One aim of our work is to build upon this pioneering research and to assess general support for ecological divergence as a driver of speciation under a wider range of ecological conditions. For example, it is likely that continental lineages seldom experience circumstances as amenable to adaptive ecological divergence as do taxa on islands -- and yet continental lineages diversify nonetheless. Given that most described species have arisen in this continental context, a critical question is to what extent adaptive ecological divergence is generally required for speciation or coexistence when lineages evolve in these more complex ecological theatres.

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

**The Sorting of Taxonomic Pairs During the Establishment of Sympatry**:
It has been suggested that taxa evolving greater ecological differences during speciation9s allopatric phase will be less likely to competitively exclude one another upon secondary contact. It has also been noted, though in a different literature, that allopatric taxa acquiring greater reproductive differences will be less likely to hybridize and fuse at that 8moment-of-truth9. Both ideas hold that taxa differ non-randomly in their ability to establish sympatry due to trait differences arising (for unrelated reasons) in allopatry. I recently synthesized these ideas into the concepts of 8ecological species sorting9 and 8reproductive species sorting9, two pre-sympatry analogs to character displacement (Anderson & Matute 2025 Ecology Letters15). I united concepts like 8differential fusion9 and 8the Templeton effect9 within these frameworks and used coexistence and assembly theories to distinguish allopatry-derived trait differences that will likely promote sympatry from those that likely will not. I finally outlined new methods that will allow researchers to test general support for each process in comparative datasets.

---

### Patterns of organismal and evolutionary reproductive isolation



### 2. Factors affecting speciation reversal

The road to origin of species is not a one-way street. While barriers to gene flow can quickly arise between lineages under some circumstances, such barriers can also quickly dissolve when circumstances change, resulting in incipient species collapse. In fact, growing evidence supporting an ephemeral speciation model ([Rosenblum et al. 2012](https://link.springer.com/article/10.1007/s11692-012-9171-x)) suggests that incipient species readily arise but are generally short-lived, and it seems likely that extinction-via-hybridization or 'speciation reversal' is a major reason. This observation points to a major consequence: to cultivate a mechanistic understanding of the build-up of biodiversity, researchers will require a much better grasp of how stable, non-ephemeral reproductive barriers tend to evolve in nature. 

In a new perspective paper, I call attention this problem and synthesize available evidence with respect to the unknown role of ecological adaptation in the evolution of unconditional or 'intrinsic' reproductive isolation [(**Anderson et al. 2023, *Am. Nat.***)](https://doi.org/10.1086/723763).

I have also launched a new research project into the evolution of intrinsic isolation between two species of wild *Drosophila* (*D. santomea and D. yakuba)*. These species form a natural hybrid zone (one of the only known for *Drosophila* in the wild) on the island of S&atilde;o Tom&eacute;, which straddles the equator off the coast of West Africa. There, the two species displace one another across an ecological gradient on the slopes of Pico de S&atilde;o Tom&eacute;, the island's highest peak, with *D. yakuba* occurring at lower elevations and the endemic *D. santomea* occupying the higher slopes. This system touches on the two major themes of my research <span>&#8212;</span> speciation and the factors affecting coexistence.

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
-->
