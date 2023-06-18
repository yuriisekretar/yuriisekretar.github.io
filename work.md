---
layout: page
title: Work
---
<ul>
  {% for work in site.work %}
    <li>
      <h2><a href="{{ work.url }}">{{ work.short_name }}</a></h2>
      <h3>{{ work.position }}</h3>
      <p>{{ work.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>
