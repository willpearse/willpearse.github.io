---
title: "Pearse Lab - Software"
layout: gridlay
excerpt: "Pearse Lab -- Software."
sitemap: false
permalink: /software/
---


# Software

{% assign number_printed = 0 %}
{% for program in site.data.software %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if program.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ program.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ program.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ program.description }}</p>
  <p><em>{{ program.authors }}</em></p>
  <p><strong><a href="{{ program.link.url }}">{{ program.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ program.news1 }}</strong></p>
  <p> {{ program.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
