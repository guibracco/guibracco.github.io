---
layout: home
title: "Projects"
permalink: /projects/
---

A collection of projects, analyses and works.

<div class="project-grid">
{% assign items = site.data.projects | sort: "sort" %}
{% for p in items %}
  <div class="project-card">
    <h3><a href="{{ p.url }}">{{ p.name }}</a></h3>
    <p>{{ p.description }}</p>

    {% if p.tags %}
    <ul class="project-tags">
      {% for t in p.tags %}
      <li>{{ t }}</li>
      {% endfor %}
    </ul>
    {% endif %}
  </div>
{% endfor %}
</div>
