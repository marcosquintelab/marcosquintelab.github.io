---
layout: default
title: People
permalink: /people/
---

# Meet the Team

<ul>
  {% for person in site.people %}
    <li>
      <strong>{{ person.name }}</strong> — {{ person.position }}  
      {% if person.image %}
        <br><img src="{{ person.image }}" alt="{{ person.name }}" style="max-height: 100px;">
      {% endif %}
      <br>{{ person.content | markdownify }}
    </li>
    <hr>
  {% endfor %}
</ul>
