---
layout: page
permalink: /archive/
title: archive
description: A place to archive all posts.
---


<hr/>
<br/>
<h2>portfolio</h2>
<br>
<ul class="post-list">
{% for project in site.portfolio %}
    <li>
        <h2><a class="poem-title" href="{{ project.url | prepend: site.baseurl }}">{{ project.title }}</a></h2>
        <p class="post-meta">{{ project.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
<hr/>
<br/>
<h2>blog</h2>
<br>
<ul class="post-list">
{% for post in site.posts %}
    <li>
        <h2><a class="poem-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
<hr/>
<br/>
<h2>poetry</h2>
<br>
<ul class="post-list">
{% for poem in site.poetry reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
