---
layout: page
title: Updates
permalink: /updates/
---

The site content below reflects the current CV dated March 18, 2026.

<ul class="update-list">
  {% for item in site.data.updates %}
  <li class="update-item">
    <span class="update-period">{{ item.period }}</span>
    <p>
      {% if item.url %}
      <a href="{{ item.url }}">{{ item.summary }}</a>
      {% else %}
      {{ item.summary }}
      {% endif %}
    </p>
  </li>
  {% endfor %}
</ul>
