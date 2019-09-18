---
title: "Pearse Lab - Team"
layout: gridlay
excerpt: "Pearse Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **If you are interested in joining the lab, see our ['join'](/join) page**

{% assign number_printed = 0 %}
{% for member in site.data.profs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><i>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  | {{ member.education1 }} |
  {% endif %}

  {% if member.number_educ == 2 %}
  | {{ member.education1 }} | {{ member.education2 }} |
  {% endif %}

  {% if member.number_educ == 3 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} |
  {% endif %}

  {% if member.number_educ == 4 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} |
  {% endif %}

  {% if member.number_educ == 5 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} | {{ member.education5 }} |
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Post-docs
{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><i>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  | {{ member.education1 }} |
  {% endif %}

  {% if member.number_educ == 2 %}
  | {{ member.education1 }} | {{ member.education2 }} |
  {% endif %}

  {% if member.number_educ == 3 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} |
  {% endif %}

  {% if member.number_educ == 4 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} |
  {% endif %}

  {% if member.number_educ == 5 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} | {{ member.education5 }} |
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.phds %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><i>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  | {{ member.education1 }} |
  {% endif %}

  {% if member.number_educ == 2 %}
  | {{ member.education1 }} | {{ member.education2 }} |
  {% endif %}

  {% if member.number_educ == 3 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} |
  {% endif %}

  {% if member.number_educ == 4 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} |
  {% endif %}

  {% if member.number_educ == 5 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} | {{ member.education5 }} |
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## MSc Students
{% assign number_printed = 0 %}
{% for member in site.data.mscs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><i>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  | {{ member.education1 }} |
  {% endif %}

  {% if member.number_educ == 2 %}
  | {{ member.education1 }} | {{ member.education2 }} |
  {% endif %}

  {% if member.number_educ == 3 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} |
  {% endif %}

  {% if member.number_educ == 4 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} |
  {% endif %}

  {% if member.number_educ == 5 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} | {{ member.education5 }} |
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Undergraduate students
{% assign number_printed = 0 %}
{% for member in site.data.ugs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {{ member.info }}<br><i>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  | {{ member.education1 }} |
  {% endif %}

  {% if member.number_educ == 2 %}
  | {{ member.education1 }} | {{ member.education2 }} |
  {% endif %}

  {% if member.number_educ == 3 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} |
  {% endif %}

  {% if member.number_educ == 4 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} |
  {% endif %}

  {% if member.number_educ == 5 %}
  | {{ member.education1 }} | {{ member.education2 }} | {{ member.education3 }} | {{ member.education4 }} | {{ member.education5 }} |
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

