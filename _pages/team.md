---
title: "Allan Lab - Team"
layout: gridlay
excerpt: "Allan Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} 
  
  {% if member.github %}
  <i><a href="{{ member.github }}">Github</a>
  {% endif %}

  {% if member.website %}
  <i><a href="{{ member.github }}">Personal website</a>
  {% endif %}

  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li><a href="{{ member.educationlink1 }}"> {{ member.education1 }} </a> </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> <a href="{{ member.educationlink1 }}"> {{ member.education1 }} </a> </li>
  <li> <a href="{{ member.educationlink2 }}"> {{ member.education2 }} </a> </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
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


![]({{ site.url }}{{ site.baseurl }}/images/teampic/group-pic.jpg){: style="width: 100%; float: center; margin: 10px"}

