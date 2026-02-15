---
layout: default
title: Статьи по ML (Гварамадзе Роман)
permalink: /ml/
---

{% include nav.html %}

# ML статьи

<ul>
{% assign sorted = site.ml | sort: "date" | reverse %}
{% for post in sorted %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%d.%m.%Y" }}</small>
  </li>
{% endfor %}
</ul>
