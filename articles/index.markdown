---
layout: article
title: Articles
subtitle: Longer-form guides and thought pieces on transparent team finances.
permalink: /articles/
---

<div class="grid two">
  {% for article in site.articles %}
    <article class="info-card">
      <h3><a href="{{ article.url | relative_url }}">{{ article.title }}</a></h3>
      <p>{{ article.excerpt | strip_html | truncate: 160 }}</p>
    </article>
  {% endfor %}
</div>
