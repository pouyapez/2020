---
title: Accepted Papers
layout: page-fullwidth
permalink: /papers/
header:
  image_fullwidth: "generic-gradient.png"
---

Note that the papers below may not be the final version (yet), but may be the anonymous versions from the _review_ phase (final versions will be available by June 8th).
All papers, with their reviews and other details, are also available on [OpenReview](https://openreview.net/group?id=AKBC.ws/2020/Conference).

## Archival Papers

<ul>
{% for paper in site.data.accepted %}
    {% if paper['archival_status'] == "Archival" %}
        {% include paper.html p=paper %}
    {% endif %}
{% endfor %}
</ul>

## Non-Archival Papers

<ul>
{% for paper in site.data.accepted %}
    {% if paper['archival_status'] == "" %}
        {% include paper.html p=paper %}
    {% endif %}
{% endfor %}
</ul>