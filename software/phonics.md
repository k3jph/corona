---
id: 2856
title: Phonetic Spelling Algorithms in R
date: 2015-09-20T18:06:31-04:00
author: James Howard
layout: page
guid: https://jameshoward.us/?page_id=2856
image: phonics.jpg
---

This is the R package to support phonetic spelling algorithms in R. Several packages provide the Soundex algorithm.  However, other algorithms have been developed since Soundex that can also provide phonetic spelling and test phonetic similarity.

## Source Code

*   [GitHub Repository](https://github.com/howardjp/phonics)

## Installation

The `phonics` R package is available for download from package at [GitHub](https://github.com/howardjp/phonics). Install `phonics` via [DevTools](https://github.com/hadley/devtools): 

{% highlight r %}
devtools::install_github("howardjp/phonics")
{% endhighlight %}

The `phonics` package is developed using the [GitFlow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) development workflow. To install the development branch, use:

{% highlight r %}
devtools::install_github("howardjp/phonics", ref = "develop")
{% endhighlight %}

## Algorithms included

*   Caverphone
    *   Original Caverphone
    *   Caverphone 2
*   Cologne (Kölner)
*   Lein
*   Match Rating Approach
    *   Encoder
    *   Comparison
*   Metaphone
*   New York State Identification and Intelligence System
    *   NYSIIS
    *   Modified NYSIIS
*   Roger Root
*   Soundex
    *   Original Soundex
    *   Apache Refined Soundex
*   Statistics Canada
    *   Census Modified

## Dependencies

*   testthat
*   roxygen2
*   Rcpp
*   BH

## Contribution guidelines

*   Use [GitFlow](http://nvie.com/posts/a-successful-git-branching-model/)
*   Write unit tests using [testthat](https://github.com/hadley/testthat)
*   Document functions using [roxygen2](https://github.com/yihui/roxygen2)

## Blog Posts

{% include relatedposts.html tag="phonics" %}

_Image by [Unsplash / Pexels](https://www.pexels.com/photo/letters-metal-typography-31323/). This work used the Extreme Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number ACI-1548562. In particular, it used the Comet system at the San Diego Supercomputing Center (SDSC) through allocations TG-DBS170012 and TG-ASC150024._