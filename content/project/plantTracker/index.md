---
title: "plantTracker: An R package to translate maps of plant occurrence into demographic data"
subtitle: "This project is a collaboration with Peter Adler, Shannon Albeke, David Atkins, Jared Studyvin and Daniel Laughlin, with funding from Wyoming EpSCOR and WEST Ecosystems Technology."
excerpt: "This R package was designed to transform long-term quadrat maps that show plant occurrence and size into demographic data that can be used to answer questions about population and community ecology."
date: 2023-03-21
author: "Alice Stears"
draft: false
#tags:
  #- hugo-site
categories:
  - Publications
  - software
#layout options: single-sidebar
layout: single
links:
- icon: door-open
  icon_pack: fas
  name: paper
  url: https://doi.org/10.1111/2041-210X.13950
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/aestears/plantTracker
---

          
 Long-term demographic data are rare yet invaluable for conservation, management, and basic research on the underlying mechanisms of population and community dynamics. Historical and contemporary mapped datasets of plant location and basal area present a relatively untapped source of demographic records that, in some cases, span over 20 years of sequential data collection. However, these maps do not uniquely mark individual plants, making the process of collecting growth, survival, and recruitment data difficult.

Recent efforts to translate historical maps of plant occurrence into shapefiles make it possible to use computer algorithms to track individuals through time and determine individual growth and survival. plantTracker is an R package which contains user-friendly functions to extract neighbourhood density, growth, and survival data from repeatedly-sampled maps of plant location and basal area. These functions can be used with data derived from quadrat maps, aerial photography, and remote sensing, and while designed for use with perennial plants, can be applied to any repeatedly mapped sessile organism.

This package contains two primary functions: 

- **trackSpp()**, which tracks individuals through time and assigns demographic data

{{< figure src="trackSppSlide.jpg" alt="A diagram of how the trackSpp() function works"
          style=" width: 800px" >}}
          
- **getNeighbors()**, which calculates both within and between-species neighbourhood occupancy around each mapped individual

{{< figure src="getNeighborsSlide.jpg" alt="A diagram of how the getNeighbors() function works"
          style=" width: 800px" >}}
          
 plantTracker also contains functions to estimate plot-level recruitment, calculate plot-level population growth rate, and create quadrat maps. 


--------------------

### Find out more about this R package...
- on [GitHub](https://github.com/aestears/plantTracker)
- on the package [webpage](astearsresearch.com/plantTracker)
- in our [paper](https://doi.org/10.1111/2041-210X.13950) published in Methods in Ecology and Evolution in 2022 

<script type='text/javascript' style="float: left;" src='https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js'></script>
<div data-badge-popover="right" data-badge-type="donut" style="float: left; margin:10px"  data-doi="doi.org/10.1111/2041-210X.13950" data-hide-no-mentions="true" class="altmetric-embed"></div>

Stears, Alice E., Peter B. Adler, Shannon E. Albeke, David H. Atkins, Jared Studyvin and Daniel C. Laughlin. 2022. plantTracker: An R package to translate maps of plant occurrence into demographic data. *Methods in Ecology and Evolution,* **13**(10), 2129-2137. [doi.org/10.1111/2041-210X.13950
]( https://doi.org/10.1111/2041-210X.13950
)