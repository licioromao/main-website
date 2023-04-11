---
layout: page
title: Publications
permalink: /publications/
nav: true
description: 
years:
nav_order: 2
---

Please find below a list of my publications.

<!-- _pages/publications.md -->

### Technical reports

<div class="publications">

{% bibliography --query @report[year=2023] %}

</div>

### Journal 

<div class="publications">

{% bibliography --query @article %}

</div>


### Conferences

<div class="publications">

{% bibliography --query @inproceedings %}

</div>

## Theses 

### DPhil (PhD) thesis

<div class="publications">

{% bibliography --query @*[key = Romao21] %}

</div>

### Master thesis (In Portuguese)

<div class="publications">

{% bibliography --query @*[key = Romao17] %}

</div>

