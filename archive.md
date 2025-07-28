---
layout: page
title: Archive
permalink: /archive/
---

<div class="post-list">
{% for post in site.posts %}
  <div class="post-item">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </div>
{% endfor %}
</div>
