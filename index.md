---
layout: default   # Use a simple default layout or create _layouts/default.html later
title: Home
---

# Welcome to Vishnu's Blog

Automated posts on latest news, health, tech, lifestyle & Kerala/India insights.

## Latest Posts

<ul>
  {% for post in site.posts limit:10 reversed %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>

New posts added automatically via Telegram bot. Check back soon!
