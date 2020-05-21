---
title: Invited Speakers
layout: page-fullwidth
permalink: /speakers/
header:
  image_fullwidth: "generic-gradient.png"
---

{% for speaker in site.data.invited-talks %}

<div id="{{ speaker.id }}Summary"></div>
<div class="row">
	<div class="large-1 columns"></div>
	<div class="small-8 medium-3 columns">
	  <img src="{{ site.baseurl }}/assets/img/people/{{ speaker.thumbnail}}"  alt="{{ speaker.name }}" style="width: 300px" />
	</div>

<div class="small-12 medium-9 large-7 columns" markdown="1">

### [{{ speaker.name }}]({{ speaker.url }})

#### {{ speaker.location }}

<br />
_{{ speaker.title }}_ <br />

<a href="#{{ speaker.id }}Detail"> Abstract and Bio</a>

</div>

<div class="large-1 columns"></div>
</div>

{% endfor %}

<br />
<br />
<br />
<h1> Speaker abstracts and bios </h1>
<hr/>
{% for speaker in site.data.invited-talks %}

<div id="{{ speaker.id }}Detail"></div>
<div class="row">
	<div class="large-1 columns"></div>
	<div class="small-8 medium-3 columns">
	  <img src="{{ site.baseurl }}/assets/img/people/{{ speaker.thumbnail}}"  alt="{{ speaker.name }}" style="width: 300px" />
	</div>

<div class="small-12 medium-9 large-7 columns" markdown="1">

### [{{ speaker.name }}]({{ speaker.url }})

#### {{ speaker.location }}

</div>
</div>
<div class="row">
<div class="large-1 columns"></div>
<div class="large-10 medium-12 columns" markdown="1">
<h4>{{ speaker.title }}</h4>
{{ speaker.abstract }}
<br /> <br />
<h6> Bio </h6>
{{ speaker.bio }}

<a href="#{{ speaker.id }}Summary">Back</a>

<hr />
</div>
<div class="large-1 columns"></div>
</div>

{% endfor %}
