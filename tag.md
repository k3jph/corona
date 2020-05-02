---
layout: page
title: Most Common Tags 
permalink: /tag
description: The topics on JamesHoward.us
sitemap:
  exclude:      yes
---

<div class="page">
   <div class='tag-cloud'>
      {% tag_cloud font-size: 50 - 300%, threshold: 10%}
   </div>

   <h1>All Posts by Tag</h1>

   {% comment %} Creates an empty array {% endcomment %}
   {% assign tags = "" | split:"" %}

   {% comment %}Creates an array of tags names{% endcomment %}
   {% for t in site.tags %}
      {% assign tags = tags | push: t[0] %}
   {% endfor %}

   {% assign sorted_tags = tags | sort_natural %}

   {% for tag in sorted_tags %}
      {% capture tagslug %}{{ tag | slugify }}{% endcapture %}
      <h2><a name="{{tagslug}}"></a>{{tag}}</h2>
      {% for post in site.tags[tag] %}
         <p><a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
         <span class="post-date">{{ post.date | date_to_string }}</span></p>
      {% endfor %}
   {% endfor %}
   </div>
