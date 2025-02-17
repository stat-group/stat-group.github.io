---
title: "Stat Group - Students and Postdocs"
layout: gridlay
excerpt: "Stat Group: Students and Postdocs"
sitemap: false
permalink: /students_and_postdocs/
---

## Prospective PhD Students

If you are interested in our Statistics and Data Science Ph.D. program, please see [here](https://uscstats.github.io/) for how to apply, application deadlines, and Zoom information session details and also check out the Ph.D. [brochure](https://www.dropbox.com/s/23wdcz1h3wbaptm/PhD-Statistics-Brochure.pdf?dl=0). Questions about the Ph.D. program can be directed to the current coordinator Gourab Mukherjee (gourab@usc.edu).

## Current PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden"> </ul>
  <ul> {{ member.education1 }} </ul>
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

## Current Postdocs
{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden"> </ul>
  <ul> {{ member.education1 }} </ul>
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

