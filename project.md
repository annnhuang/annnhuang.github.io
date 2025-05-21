---
layout: default
title: Projects
permalink: /projects/
---

## Projects

<ul class="project-list">
  {% for project in site.projects %}
    <li>
      <a href="{{ project.url }}">{{ project.title }}</a><br>
      <small>{{ project.description }}</small>
    </li>
  {% endfor %}
</ul>
