---
layout: blog
title: Blog
subtitle: Tips, updates, and season-ready financial guidance for minor hockey treasurers.
permalink: /blog/
---

<div class="grid two">
  {% for post in site.posts %}
    <article class="info-card">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="muted">{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </article>
  {% endfor %}
</div>
