---
layout: single
title: "Conferences & Seminars"
permalink: /conferences/
author_profile: true
---

## Upcoming
{% for c in site.data.conferences.upcoming %}
- {% if c.link %}**[{{ c.title }}]({{ c.link }})**{% else %}**{{ c.title }}**{% endif %} — {{ c.location }}.  
  *{{ c.when }}*
{% endfor %}

## Past conferences and seminars
{% for group in site.data.conferences.past %}
### {{ group.track }}
{% for c in group.items %}
- {% if c.link %}**[{{ c.title }}]({{ c.link }})**{% else %}**{{ c.title }}**{% endif %} — {{ c.location }}.  
  *{{ c.when }}*
{% endfor %}
{% endfor %}
