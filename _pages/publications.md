---
layout: page
permalink: /publications/
title: Publications
description: Artificial Intelligence, Material Science.
years: [2022, 2023, 2024, 2025, 2026, 2027, 2028]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
