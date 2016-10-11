---
layout: page
permalink: /sitemap/
title: SITEMAP
description: 
---

<ul class="post-list">
{% for page in site.pages %}
    {% unless page.title == "SITEMAP" %}
        <!-- initial for loop content goes here-->
    <li>
        <h2><a class="poem-title" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></h2>
        <p class="post-meta">{{ page.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
       {% endunless %}
{% endfor %}
</ul>

