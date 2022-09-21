---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [2022,2021,2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
