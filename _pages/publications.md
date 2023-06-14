---
layout: page
permalink: /publications/
title: publications
description:  
years: [2023, 2022, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<p>An up-to-date list is available on <a href="https://scholar.google.com/citations?user=aEcQu2EAAAAJ&hl=en" target="_blank" rel="noopener noreferrer">Google Scholar</a>.</p>

<p>* denotes equal contribution.</p>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
