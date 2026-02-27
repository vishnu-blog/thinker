---
layout: default
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
  {% empty %}
    <li>No posts yet — new ones added automatically via Telegram bot!</li>
  {% endfor %}
</ul>

<p>New posts added automatically via Telegram bot. Check back soon!</p>
