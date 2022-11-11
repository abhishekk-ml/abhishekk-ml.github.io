---
layout: page
permalink: /research/
title: Research
description: 

years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2013, 2012, 2011, 2010, 2009, 2008]
topics: [Distribution or task shift, Generative models, Matrix factorization, Inducive bias, Multitask learning, Multi-modal learning, Deep learning (other)]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
An up-to-date list of my papers is available on <a href="https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en" target="_blank" rel="noopener noreferrer">Google Scholar</a>. For publications loosely grouped by topics, <a href="#pub-by-topics">see here</a>. 
<h1>Publications (by year)</h1>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>


<div class="publications">
<h1 id="pub-by-topics">Publications (by topic)</h1>
{%- for t in page.topics %}
  <h2 class="topic">{{t}}</h2>
  {% bibliography -f papers -q @*[topic={{t}}]* %}
{% endfor %}

</div>
