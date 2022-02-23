---
layout: page
permalink: /publications/
title: publications
description: A complete list of my research publications. Including pre-prints.
years: [2022, 2021, 2019]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
