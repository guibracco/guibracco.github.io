---
layout: page
title: "Projects"
permalink: /projects/
---

<div class="project-grid">
{% for p in site.data.projects %}
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
