---
layout: default
title: Projects
---
## My Projects

<ul style="list-style: none; padding: 0;">
  {% for project in site.projects %}
    <li style="margin-bottom: 20px; padding-bottom: 10px; border-bottom: 1px solid #555;">
      <h3 style="margin-bottom: 5px;"><a href="{{ project.url | relative_url }}" style="text-decoration: none;">{{ project.title }}</a></h3>
      {% if project.date %}
        <p style="font-size: 0.9em; color: #bbb; margin-top: 0;">{{ project.date | date_to_string }}</p>
      {% endif %}
      <p>{{ project.description | default: project.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
