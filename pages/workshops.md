---
title: Workshops
layout: page-fullwidth
permalink: /workshops/
header:
  image_fullwidth: "irvine-header.jpg"
---

<ul>
{% for organizer in site.data.workshops %}
    <li>
    <b>{{ organizer.acronym}}: {{ organizer.name }}</b>
    <br>
    {{ organizer.organizers }}
    <br>
    <a href="{{ organizer.url }}">Website</a>
    </li>
{% endfor %}
</ul>

If you have any questions, please get in touch with our workshop chairs.
