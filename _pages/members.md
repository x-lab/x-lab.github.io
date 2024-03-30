---
title: "X-Lab - members"
layout: gridlay
excerpt: "X-Lab: Team members"
sitemap: false
permalink: /members/
---

# Members of XLab

**We are looking for passionate staff engineers and scientists, postdoctorial fellows, graduate and undergraduate students/interns to [join our team]({{ site.url }}{{ site.baseurl }}/join)!**

<!-- Jump to [staff](#staff), [students](#students), [interns](#interns), and [administrative support](#administrative-support). -->
<hr />
## PI
{% for member in site.data.pi %}

  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>

  <ul style="overflow: hidden">
    <li> {{member.title1}} </li>
    <li> {{member.title2}} </li>
    <li> {{member.title3}}</li>
  </ul>

{% endfor %}

<hr />
## Staff
{% assign number_printed = 0 %}
{% for member in site.data.staff %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <!-- <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> -->
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education4 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education5 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
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

<hr />

## Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <!-- <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> -->
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
    <li> {{ member.education3 }} </li>
    <li> {{ member.education2 }} </li>
    <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education4 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education5 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
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

<hr />

## Interns
{% assign number_printed = 0 %}
{% for member in site.data.interns %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education4 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education1 }} </li>
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


<!--
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
{% endif %} -->

<hr />

## Alumni
<div class="row">
  <div class="col-sm-6 clearfix">
  <h4>Staff</h4>
  {% for member in site.data.alumni_visitors %}
  {{ member.name }}
  {% endfor %}
  </div>

  <div class="col-sm-6 clearfix">
  <h4>Interns</h4>
  {% for member in site.data.alumni_msc %}
  {{ member.name }}
  {% endfor %}
  </div>
</div>

<hr />
