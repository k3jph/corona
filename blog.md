---
layout:         page
title:          Blog
menu-order:     1
menu-label:     Blog
sitemap:
  exclude:      yes
---

<div class="page">
  {% comment %}
    Yes, I am about to introduce a Y10k problem.  I figure there is
    plenty of time to fix it later.
  {% endcomment %}
  {% assign currentyear = 10000 %}
  {% for post in site.posts %}
    {% capture postyear %}{{ post.date | date: "%Y" }}{% endcapture %}
    {% if postyear != currentyear %}
      {% assign currentyear = postyear %}
      <h2><a name="{{ currentyear | slugify }}"></a>{{ currentyear }}</h2>
    {% endif %}
    <p><a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date_to_string }}</span></p>
  {% endfor %}
</div>
