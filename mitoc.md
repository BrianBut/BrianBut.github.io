---
layout: default
---

<div class="container">
    <h1><b>Memories In the Time of Covid</b></h1>
    {% assign pages = site.pages | sort: eventDate %}
    {% for page in pages %}
      {% if page.published %}
        {% if page.category == 'mitoc' %}
        <li>
            <a href="{{ page.url }}">{{ page.title }} {{ page.eventDate }}</a>
        </li>
        {% endif %}
      {% endif %}
    {% endfor %}
</div>


