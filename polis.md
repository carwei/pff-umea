---
layout: default
title: Polistillstånd
---

<h1>PDF Files</h1>
<ul>
  {% for file in site.static_files %}
    {% if file.path contains '/assets/permits/' %}
      <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
