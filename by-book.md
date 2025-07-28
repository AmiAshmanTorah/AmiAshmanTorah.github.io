---
layout: page
title: By Book
permalink: /by-book/
---

## Torah
{% assign torah_posts = site.posts | where_exp: "post", "post.categories contains 'Torah'" %}
{% for post in torah_posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.book }} {{ post.hebrew_ref }}
{% endfor %}

## Nevi'im
{% assign neviim_posts = site.posts | where_exp: "post", "post.categories contains 'Neviim'" %}
{% for post in neviim_posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.book }} {{ post.hebrew_ref }}
{% endfor %}

## Ketuvim
{% assign ketuvim_posts = site.posts | where_exp: "post", "post.categories contains 'Ketuvim'" %}
{% for post in ketuvim_posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.book }} {{ post.hebrew_ref }}
{% endfor %}
