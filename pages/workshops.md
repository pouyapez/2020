---
title: Workshops
layout: page-fullwidth
permalink: /workshops/
header:
  image_fullwidth: "generic-gradient.png"
---

Workshops will take place on **June 25, 2020** from 8am-1pm, PT.

<ul>
{% for workshop in site.data.workshops %}
    <li>
    <b>
        {{- workshop.title -}}
        {% if workshop.acronym %}
            ({{- workshop.acronym -}})
        {%- endif -%}
    </b>, <i>{{- workshop.duration -}}</i>
    {%- if workshop.url -%}
    , <a href="{{ workshop.url }}">Website</a>
    {%- endif -%}
    {%- if workshop.authors -%}
    <br>
    <i>
        {{- workshop.authors | join: ", " -}}
    </i>
    {%- endif -%}
    </li>
{% endfor %}
</ul>

If you have any questions, please get in touch with our workshop chairs.
