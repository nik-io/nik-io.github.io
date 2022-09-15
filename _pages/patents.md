---
layout: page
permalink: /patents/
title: patents
#description: patents by categories in reversed chronological order. generated by jekyll-scholar.
years: [2022,2021,2020,2019,2018,2017,2016,2015]
nav: true
nav_order: 3
---
<!-- _pages/patents.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>