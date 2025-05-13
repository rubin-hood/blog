---
layout: home        # Minima hat ein „home“-Layout, das site.posts rendert
title: Blog
permalink: /blog/
---

# {{ page.title }}

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      – {{ post.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
