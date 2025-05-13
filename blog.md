---
layout: default       # oder: home, wenn dein Theme das unterstützt
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
