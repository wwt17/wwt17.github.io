---
layout: page
permalink: /publications/
title: publications
description: and on-going works
kinds: ["In prep.", "2024", "2023", "Older"]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for kind in page.kinds %}
  <h2 class="year">{{kind}}</h2>
  {% bibliography -f papers -q @*[kind={{kind}}]* %}
{% endfor %}

</div>
