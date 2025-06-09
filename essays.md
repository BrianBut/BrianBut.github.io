---
layout: default
---

<div class="w3-container">
    <h1><b>Essays</b></h1>
    {% for page in site.pages %}
      {% if page.published %}
        {% if page.category == 'essay' %}
        <li>
            <a href="{{ page.url }}">{{ page.title }} {{ page.eventDate }}</a>
        </li>
        {% endif %}
      {% endif %}
    {% endfor %}
</div>
