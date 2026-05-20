---
layout: default
title: Blog
description: Insights from the adversarial perspective.
permalink: /blog/
---

<section class="page-hero">
  <div class="container">
    <span class="kicker">Blog</span>
    <h1>Insights from the adversarial perspective.</h1>
    <p>Analysis on attack paths, flawed assumptions, trust relationships, and the quiet failure modes inside security programs.</p>
  </div>
</section>

<section class="section">
  <div class="container post-list">
    {% for post in site.posts %}
    <article class="post-card">
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt | strip_html | truncate: 220 }}</p>
    </article>
    {% endfor %}
  </div>
</section>
