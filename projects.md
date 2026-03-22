---
layout: page
title: "Projects"
permalink: /projects/
---

{% for p in site.data.projects %}
### [{{ p.name }}]({{ p.url }})

{{ p.description }}

{% if p.tags %}
**Tags:** {{ p.tags | join: ", " }}
{% endif %}

---
{% endfor %}
