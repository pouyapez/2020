---
title: Workshops
layout: page-fullwidth
permalink: /workshops/
header:
  image_fullwidth: "generic-gradient.png"
---

Workshops will take place on **June 25, 2020** from 8am-1pm, PT.

<div>
{% for workshop in site.data.workshops %}
    <h3>
        {{- workshop.title -}}
        {% if workshop.acronym %}
            ({{- workshop.acronym -}})
        {%- endif -%}
    </h3>
    <!-- , <i>{{- workshop.duration -}}</i> -->
    {%- if workshop.authors -%}
    <span class="subheadline">
        {{- workshop.authors | join: ", " -}}
    </span>
    {%- endif -%}
    <br/>
    {%- if workshop.url -%}
    <a class="button grey" href="{{-workshop.url-}}">Website</a>
    {%- endif -%}
    <a class="button" href="https://akbc.apps.allenai.org/workshop_{{- workshop.UID -}}.html">Live Event</a>
{% endfor %}
</div>

If you have any questions, please get in touch with our workshop chairs.
