---
layout: page
title: Blog
description: Write-ups, vulnerability research, and tool walkthroughs.
permalink: /blog/
---

{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts %}
  <li class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <div class="post-date">{{ post.date | date: "%Y-%m-%d" }}</div>
    {% if post.excerpt %}
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 200 }}</p>
    {% endif %}
    {% if post.tags %}
    <div class="card-tags" style="margin-top: 0.3rem;">
      {% for tag in post.tags %}
      <span class="tag">{{ tag }}</span>
      {% endfor %}
    </div>
    {% endif %}
  </li>
  {% endfor %}
</ul>
{% else %}
<div class="placeholder">Write-ups coming soon — CVE research, bug bounty methodology, and tool deep dives.</div>
{% endif %}
