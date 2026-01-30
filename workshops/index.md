---
layout: default
title: "Workshops"
description: "Details of ICT workshops and sessions"
permalink: /workshops/
---

# Workshops & Sessions

Below are workshops and session posts. This page automatically lists posts with the tag `workshop`.

<ul class="workshop-list">
{% assign workshop_posts = site.posts | where_exp:"post","post.tags contains 'workshop'" %}
{% for post in workshop_posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="meta"> — {{ post.date | date: "%Y-%m-%d" }}</span>
    {% if post.excerpt %}<p>{{ post.excerpt }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

If you prefer to use a category instead of a tag, replace the filter with:
{% raw %}{% assign workshop_posts = site.posts | where:"category","workshop" %}{% endraw %}
