---
layout: default
title: Статьи по SEO (Гварамадзе Роман)
permalink: /seo/
---

# SEO статьи

<ul>
{% assign sorted = site.seo | sort: "date" | reverse %}
{% for post in sorted %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%d.%m.%Y" }}</small>
  </li>
{% endfor %}
</ul>
