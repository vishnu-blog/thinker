---
layout: default   # This tells Jekyll to use a layout (create _layouts/default.html if missing)
title: Home
---

# Welcome to Vishnu's Blog

Automated posts on latest news, health, tech, lifestyle & Kerala/India insights.

## Latest Posts

<ul>
  {% for post in site.posts reversed %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

<p>New posts added automatically via Telegram bot. Check back soon!</p>
