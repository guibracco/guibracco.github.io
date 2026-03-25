---
layout: home
title: "Home"
---

I build **AI-first data tooling**: agents, workflows, and apps that help teams go from raw data → insights faster.

## Featured projects

<div class="project-grid">
{% assign featured = site.data.projects | where: "featured", true | sort: "sort" %}
{% for p in featured %}
  <div class="project-card">
    <h3><a href="{{ p.url }}">{{ p.name }}</a></h3>
    <p>{{ p.description }}</p>
  </div>
{% endfor %}
</div>

See all projects on the [Projects](/projects/) page.
