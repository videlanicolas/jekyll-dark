---
layout: default
title: Blog
---
## Latest Posts

<ul style="list-style: none; padding: 0;">
  {% for post in site.posts %}
    <li style="margin-bottom: 20px; padding-bottom: 10px; border-bottom: 1px solid #555;">
      <h3 style="margin-bottom: 5px;"><a href="{{ post.url | relative_url }}" style="text-decoration: none;">{{ post.title }}</a></h3>
      <p style="font-size: 0.9em; color: #bbb; margin-top: 0;">{{ post.date | date_to_string }}</p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
