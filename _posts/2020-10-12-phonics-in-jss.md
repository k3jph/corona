---
id: phonics-in-jss
title: Phonics in JSS
date: 2020-10-12T11:59:00-04:00
author: k3jph
layout: post
guid: 
permalink: /2020/10/12/phonics-in-jss
image: /assets/images/phonics-in-jss.jpg
categories:
  - Blog
tags:
  - phonics
  - articles
  - R
---

I am very happy to say my new article, ["Phonetic Spelling Algorithm
Implementations for R," was published in the _Journal of Statistical
Software_](https://www.jstatsoft.org/article/view/v095i08), this morning.  
This article is the culmination of a few
years of work, off-and-on, working with phonetic spellign algorithms
for [record linkage](https://hdsr.mitpress.mit.edu/pub/8fm8lo1e/release/2).
The package supports a wide variety of historical and current phonetic
spelling algorithms:

* Caverphone
  * Original Caverphone
  * Caverphone 2
* Cologne (Kölner)
* Lein
* Match Rating Approach
  * Encoder
  * Comparison
* Metaphone
* New York State Identification and Intelligence System
  * NYSIIS
  * Modified NYSIIS
* Oxford Name Compression Algorithm
* Phonex
* Roger Root
* Soundex
  * Original Soundex
  * Apache Refined Soundex
* Statistics Canada
  * Census Modified

It's been pleasing to see an occasional user send me an email because they
been putting it to use.  It all started because I needed a high-speed
soundex and I just let it grow from there.  This yak may not be shaved
yet.  Maybe a
[version in Rust, next...](https://github.com/k3jph/phonics-in-rust)
