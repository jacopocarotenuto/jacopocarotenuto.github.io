---
layout: page
permalink: /publications/
title: My Plublication
description: You can see here all my publication! A little empty now, but prepared for the future!
years: []
nav: false
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
