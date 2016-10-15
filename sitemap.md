---
layout: page
permalink: /sitemap/
title: SITEMAP
description: 
---

<ul class="post-list">
{% for page in site.pages %}
     {% if page.sitemap == 'main' %}
        <!-- initial for loop content goes here-->
    <li>
        <h2><a class="poem-title" href="{{ page.url | prepend: site.baseurl }}">{{ page.title | capitalize }}</a></h2>
      <p class="post-meta">{{ page.description }}</p>
      </li>
       {% endif %}
{% endfor %}
</ul>
