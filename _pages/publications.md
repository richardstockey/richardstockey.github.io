---
layout: page
permalink: /publications/
title: publications
description: Peer-reviewed publications in reversed chronological order.
nav: true
nav_order: 1
years: [2024,2023,2022,2021,2020,2018]
---
Please <a href="mailto:r.g.stockey@soton.ac.uk">email</a> me if you do not have institutional access to a paper (or papers) that you would like to read!

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>