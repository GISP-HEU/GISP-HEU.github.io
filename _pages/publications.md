---
layout: page
permalink: /publications/
title: Publications
description: Note * denotes corresponding author
journal_years: [2023, 2022, 2021, 2020, 2019, 2018]
conf_year: [2023, 2022, 2021, 2020, 2019, 2018]
arxiv_years: [2023, 2021, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h1> 期刊论文-Journal Papers </h1>
{%- for y in page.journal_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journal -q @*[year={{y}}]* %}
{% endfor %}

<h1> 会议论文-Conference Papers </h1>
{%- for y in page.journal_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conference -q @*[year={{y}}]* %}
{% endfor %}

<h1> 预印-Preprints </h1>
{%- for y in page.arxiv_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f arxiv -q @*[year={{y}}]* %}
{% endfor %}

</div>
