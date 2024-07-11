---
title: Research
layout: page
---

### Atmospheres and evolution of Very Massive Stars (VMS)
*Updated July 2024*

In the theme of my main research combining evolution models with atmosphere models, I am currently focussing on stars of more than 100 solar masses, the so-called very massive stars (VMS). Albeit few in number, these stars are so luminous that some of their spectral features can dominate the observed spectra of entire stellar populations (for example the HeII-4686 emission line in the R136 cluster). 

Currently, I am post-processing stellar evolution tracks computed with GENEC by connecting the resulting stellar structure to a detailed atmosphere model computed with PoWR. Unconventionally, we compute these atmosphere models to an optical depth of up to 2000 in order to include the iron opacity peak located beneath the surface at ~200kK. Questions we hope to address are:

- How does the iron opacity peak affect the atmospheric structure? Does it change the synthesized spectrum despite its high optical depth?

- How does the atmosphere evolve throughout the main sequence of very massive stars and what spectral imprint does it leave?

- When and how do very massive stars transition from O-type to WNh-type spectra?

- How can we use the findings from detailed atmosphere models to correct the surface conditions approximated by stellar evolution models?

I presented some preliminary results at the [POEMS 2024](https://stel.asu.cas.cz/MassiveStars2024/) conference in Rio de Janeiro, the slides for which are available [here](https://jorisjosiek.com/assets/documents/202406-Talk.pdf).

___

### Benchmarking stellar evolution codes
*Updated July 2024*

As part of the [XshootU](https://massivestars.org/xshootu/) collaboration, I am involved in a project that aims to compare results computed with different widely-used stellar evolution codes (MESA, GENEC, ...) when applied to the analysis of massive stars. We aim to calibrate these codes with each other and use them to obtain evolutionary parameters (such as mass, age, rotation rate, etc.) of several stars that were analyzed spectroscopically in the XShootU dataset. Our main goal is to establish the systematic inconsistencies between the different evolution codes and identify their main uncertainties when applied to massive star research.

___

### Ph.D. project

*The following is the official preliminary title and abstract of my Ph.D. project as submitted to the International Max-Planck Research School for Astronomy at the University of Heidelberg ([IMPRS-HD](https://www.imprs-hd.mpg.de/506805/Josiek-Joris)).*

**Towards a joined picture of evolved massive stars: combining insights from stellar structure and evolution modelling.**

Through their powerful winds and large radiative output, massive stars play a central role in shaping the world around them. They are the only sources of heavy elements, many of which are essential to our life on Earth, and their strong ionizing flux is thought to be a possible driver of cosmic reionization, the last major phase transition of the universe. 

In order to understand the impact of massive stars in the universe, one needs accurate models of their evolution across time, which is achieved using codes specialized in stellar evolution. However, one major shortcoming of all stellar evolution codes is their lack of a physically consistent atmosphere including detailed raditative transfer, rendering these codes unable to predict stellar spectra, electronic population numbers, atmospheric temperature stratification or mass loss rates, which are vital quantities for interpreting observations and for computing the evolution itself. These problems are then typically solved by using separate codes which use a distinct set of physical and numerical assumptions to compute a detailed stellar atmosphere. 

Despite the fact that stellar evolution and stellar atmospheres are modeled separately, their deep interconnectedness in massive stars hints at possible benefits of a more unified approach. It is the goal of my PhD to investigate this possibility further, and establish links between these two modeling techniques. I will use the Geneva stellar evolution code (GENEC) to compute models of massive stars and then compare the computed stellar structure to the output of detailed atmosphere models using the Potsdam Wolf-Rayet stellar atmospheres code (PoWR). The first steps will involve identifying discrepancies between the predictions of the two codes, understanding their underlying origin, and using this knowledge to establish a more accurate way to incorporate results from evolution and atmosphere models. Ultimately, the long-term aim of this endeavor will be to create an interface between the two codes that would enable us to join the evolutionary and the atmospheric codes into a single, simultaneous and physically consistent computation.
