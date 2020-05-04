---
id: 3825
title: Waterfall Charts in R
date: 2016-02-15T21:20:44-05:00
author: James Howard
layout: page
guid: https://jameshoward.us/?page_id=3825
ampforwp-amp-on-off:
  - default
image: /assets/images/waterfall.jpg
---
The waterfall chart was originally introduced to the public by Ethan Rasiel in _[The McKinsey Way](http://www.amazon.com/The-McKinsey-Way-Ethan-Rasiel/dp/0070534489)_ as a way of illustrating the value of simple and understandable charts. These charts show how a collection of data points contribute to a summary total. Two common applications for waterfall charts come from financial data. The first takes a collection of financial panel data, such as a balance sheet, and shows how each component, such as different asset and liability classes, chance the final balance. The second uses financial time series data, such as annual profit-and-loss data for an organization, to demonstrate how changes year over year contribute to a final total, such as a net asset balance.

## Source Code

* [GitHub Repository](https://github.com/howardjp/waterfall)

## Installation
The `waterfall` R package is available for download from package at [GitHub](https://github.com/howardjp/waterfall).  Install `waterfall` via [DevTools](https://github.com/hadley/devtools):

{% highlight r %}
devtools::install_github("howardjp/waterfall")
{% endhighlight %}

The `waterfall` package is developed using the [GitFlow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) development workflow.  To install the development branch, use:

{% highlight r %}
devtools::install_github("howardjp/waterfall", ref = "develop")
{% endhighlight %}

## Dependencies

* lattice

## Contribution guidelines

* Use [GitFlow](http://nvie.com/posts/a-successful-git-branching-model/)
* Document functions using [roxygen2](https://github.com/yihui/roxygen2)

## Blog Posts

{% include relatedposts.html tag="waterfall" %}

_Image by [Unsplash / Pexels](https://www.pexels.com/photo/waterfall-river-summer-swimming-26430/)._
