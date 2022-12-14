---
layout: page
permalink: /publications/
title: publications
description: Peer-reviewed publications in reversed chronological order.
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

Please <a href="mailto:r.g.stockey@soton.ac.uk">email</a> me if you do not have institutional access to a paper (or papers) that you would like to read!
