---
title: "Using git, GitHub, and R Studio"
weight: 1
subtitle: "Learning and practicing how to use git, GitHub, and R Studio to collaborate with yourself and others. Here are materials and information for a workshop on this topic held on April 14th, 2023 as part of the UW R-Ladies Group. "
#excerpt: "git and GitHub are great tools."
date: 2023-04-06
draft: false
links:
#- icon: door-open
#  icon_pack: fas
#  name: website
#  url: https://bakeoff.netlify.com/
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/Rladies-uwyo/Code-Share
- icon: images
  icon_pack: fas
  name: slides
  url: https://aestears.quarto.pub/git-github-and-r-studio/#/title-slide
---
## Workshop Slides are [Here](https://aestears.quarto.pub/git-github-and-r-studio/#/title-slide) 

## Pre-Workshop To-Do

#### We're so excited to talk and learn about git, GitHub and R Studio with you on April 14th! In order to streamline the interactive part of the workshop, here are a few tasks you should complete before our meeting. I bet many of you have already completed at least a few of them, so it shouldn't take long to finish the list! 

### 1. Download R and R Studio
I imagine most folks have already completed this step, but just in case you haven't, download *both* programs at these links: 

* R : [https://cran.rstudio.com/](https://cran.rstudio.com/)

* R Studio: [https://posit.co/download/rstudio-desktop/#download](https://posit.co/download/rstudio-desktop/#download)

Even if you already use R and R Studio, you should take this as an opportunity to check that you're running current versions of both programs. It's generally important to stay up to date with software versions, since software updates are functional! They fix known issues, keep things running smoothly, and introduce useful features. Also, the more out of date your are, the more likely it is that you'll face compatability issues with R packages and other integrations. It's also important to note that updating R Studio does *not* update R, and vice-versa. So if you think that you updated recently, it's still useful to check that you've actually updated *both* programs. 

* To check the version of R Studio you're running, use the function `RStudio.Version()` in your R Studio console. The most current version of R Studio is '2023.3.0.286'--I suggest updating it if you're far behind. Thankfully it's easy to update from inside R Studio itself. Click the "Help" button in the toolbar, then select "Check for Updates" from the dropdown menu and follow the instructions that appear. 

* To check the version of R that's downloaded on your computer, use the function `R.Version()$version.string` in your R console. "Shortstop Beagle 4.2.3" is the current full version, and the "development" version (most current, but still going through some bug fixes) is "Already Tomorrow 4.3.0". The first number of the version string indicates the "major version" (i.e. the 4 in 4.2.3). You **really** should be running R version 4, since there were significant changes that took place between major versions 3 and 4. The second number in the version string indicates the "minor version" (i.e. the 2 in 4.2.3). It's generally recommended that you stay within 1 minor version of the most current full version. So, if you're running 4.1.etc or earlier, you should really update! There are several ways to do this: 
  * You can reinstall R by following the instructions in this link [https://cran.rstudio.com/](https://cran.rstudio.com/)
  * Windows: you can use the `updateR()` function in the `installr` R package. 
  * Mac: use the `updateR()` function in the `updateR` package, which can be downloaded from GitHub with `devtools::install_github("AndreaCirilloAC/updateR")`. 

If you update major or minor R versions (rather than "patch versions," which are indicated by the last number in the version string-- going from 3.4.2 to 3.4.3 is a "patch version" update), you'll need to reinstall the R packages you'd previously installed. The Windows `installr` package does this automatically, but for other methods you need to do it yourself. It's really not too much of a headache-- you can do it on an ad-hoc basis, installing a package whenever you need to use it, or do it all at once by following directions here [https://rstats.wtf/maintaining-r.html#how-to-transfer-your-library-when-updating-r](https://rstats.wtf/maintaining-r.html#how-to-transfer-your-library-when-updating-r)

### 2. Download git
Follow the instructions at this link: [https://happygitwithr.com/install-git.html](https://happygitwithr.com/install-git.html).
Note that this process is different for eaching operating system, so be sure to follow the instructions that correspond to your machine! 

### 3. Make a free GitHub account
There are several different git clients that you can use to host remote versions of your respositories, but we're going to use GitHub. It's one of the most popular, and a free account has a majority of the features you'd ever need. If you don't already have an account, you can make one for free here [https://github.com/signup](https://github.com/signup). I'd recommend using a non-UW email so that you can still access your account easily if/when you leave UW, but it's up to you. If you already have a GitHub account, make sure you know the password and are ready to login when you get to the workshop! 

