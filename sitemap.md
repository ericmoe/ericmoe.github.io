---
layout: page
permalink: /sitemap/
title: SITEMAP
description: The map of the site
---

<ul class="post-list">
{% for page in site.pages reversed %}
    <li>
        <h2><a class="poem-title" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></h2>
        <p class="post-meta">{{ page.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>

{% for page in site.pages %}
          {% if page.title %}
          <a class="page-link" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a>
          {% endif %}
        {% endfor %}
