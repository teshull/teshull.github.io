---
layout: page
permalink: /publications/
title: Publications
years: [2021, 2020, 2019, 2018, 2017, 2014]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
