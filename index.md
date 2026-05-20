---
layout: default
title: Home
description: Strategic security insight from the attacker’s perspective.
---

<section class="hero">
  <div class="container hero-grid">
    <div>
      <span class="kicker">Strategic Adversarial Security Advisory</span>
      <h1>See your security program the way attackers do.</h1>
      <p class="lead">
        Adversarial Insights helps security leaders identify hidden attack paths, flawed assumptions, and systemic weaknesses before real attackers exploit them.
      </p>
      <div class="hero-actions">
        <a class="btn" href="/contact/">Request Assessment</a>
        <a class="btn-secondary" href="/services/">Explore Services</a>
      </div>
    </div>
    <div class="hero-panel">
      <img src="{{ '/assets/images/hero-network.png' | relative_url }}" alt="Network attack path illustration">
    </div>
  </div>
</section>

<section class="service-strip">
  <div class="container service-grid">
    <article class="card">
      <h3>Adversarial Readiness Review</h3>
      <p>A strategic assessment of your security program through the lens of a real attacker.</p>
    </article>
    <article class="card">
      <h3>Red Team Program Development</h3>
      <p>Design a red team capability aligned to business risk, validation, and executive reporting.</p>
    </article>
    <article class="card">
      <h3>Offensive Security Consulting</h3>
      <p>Bring offensive-minded clarity to your Purple Team Program, existing Offensive Security Program, or other Offensive Security tasks and projects.</p>
    </article>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-header">
      <h2>Most security failures are not caused by missing tools.</h2>
      <p>
        They happen because assumptions go unchallenged, ownership is unclear, trust boundaries are poorly understood, and detection is assumed to work rather than validated.
      </p>
    </div>
    <div class="content-grid">
      <article class="card">
        <h3>Find the hidden attack paths</h3>
        <p>Understand how a real attacker would move from initial access to critical assets across identity, cloud, and CI/CD trust relationships.</p>
      </article>
      <article class="card">
        <h3>Expose systemic weaknesses</h3>
        <p>See beyond isolated vulnerabilities and understand where teams, processes, and architecture create exploitable opportunity.</p>
      </article>
      <article class="card">
        <h3>Deliver executive clarity</h3>
        <p>Translate technical complexity into concise, strategic insight that helps leadership prioritize the risks that actually matter.</p>
      </article>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-header">
      <h2>Recent Posts</h2>
      <p></p>
    </div>
    <div class="post-list">
      {% for post in site.posts limit:3 %}
      <article class="post-card">
        <small>{{ post.date | date: "%B %d, %Y" }}</small>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
      </article>
      {% endfor %}
    </div>
  </div>
</section>
