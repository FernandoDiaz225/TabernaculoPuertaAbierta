---
layout: default
title: Sermons
permalink: /sermons/
---

<ul>
  {% assign items = site.posts | where: "category", "sermons" %}
  {% for post in items %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
