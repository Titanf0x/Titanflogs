---
layout: default
title: Home
---

## Welcome to the Vault

I am **Titanfox**. This is the nexus of my creative outputs—a sanctuary insulated from the algorithmic noise of modern social networks. Here you will find projects, short stories, essays, and reports from the field.

<hr class="ornate">

### Recent Transmissions

<div class="grid">
  {% for post in site.posts limit:4 %}
  <div class="card">
    <h4><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h4>
    <p style="font-size: 0.8rem; color: var(--metal-light);">{{ post.date | date: "%b %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncatewords: 15 }}</p>
  </div>
  {% endfor %}
</div>