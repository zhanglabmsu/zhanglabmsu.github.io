---
layout: page
permalink: /publications/
title: Publications
description:  
years: [2024, 2023, 2022, 2021, 2019, 2017, 2015, 2014, 2011, 2009]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->
<div class="test">
    <p> * = Co-first author. # = Corresponding author.</p>
</div>
For the latest, please check [Google Scholar](https://scholar.google.com/citations?hl=en&user=igqQYbgAAAAJ&view_op=list_works&sortby=pubdate).

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
