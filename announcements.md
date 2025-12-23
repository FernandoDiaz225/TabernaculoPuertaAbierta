---
layout: default
title: Announcements
permalink: /announcements/
---

<ul>
  {% assign items = site.posts | where: "category", "announcements" %}
  {% for post in items %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%b %d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
