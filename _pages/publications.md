---
layout: page
permalink: /publications/
title: Publications
description: publications by categories in reversed chronological order.
years: [2012,2013,2014,2015,2016,2018,2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
