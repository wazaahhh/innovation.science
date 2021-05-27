---
layout: page
permalink: /publications/
title: publications
description: in reverse chronological order
years: [2021,2019,2018,2017,2016,2015,2014,2013,2011,2010,2009,2008]
nav: true
nav_order: 1
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
