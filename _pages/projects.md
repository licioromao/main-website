---
layout: page
title: Research
permalink: /Research/
description: The links below contain information about some of my research projects. A non-exaustive list of collaborators and of students I have supervised are shown below. 
nav: true
nav_order: 2
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>


##### Collaborators

- [Prof. Alessadro Abate](https://www.cs.ox.ac.uk/people/alessandro.abate/home.html). University of Oxford.
- [Prof. Antonis Papachristodoulou](http://sysos.eng.ox.ac.uk/wiki/index.php/User:Antonis). University of Oxford.
- [Prof. Ashish Hota](http://www.facweb.iitkgp.ac.in/~ahota/index.html). IIT Kharagpur.
- [Prof. Kostas Margellos](https://kostasmargellos.github.io/). University of Oxford.
- [Prof. Luca Laurenti](https://www.tudelft.nl/en/staff/l.laurenti/?cHash=d00d764e03ebc8279dc6679ff1d65e18). TU Delft.
- [Prof. Manuel Mazo](https://mmazojr.3me.tudelft.nl/). TU Delft.
- [Prof. Mauricio de Oliveira](https://guitar.ucsd.edu/mauricio/). University of California, San Diego.
- [Prof. Nils Jensen](http://www.cs.ru.nl/personal/nilsjansen/). Radboud University.
- [Prof. Pedro Luis Dias Peres](https://www.fee.unicamp.br/profs/peres/). University of Campinas.
- [Prof. Raphael Jungers](https://perso.uclouvain.be/raphael.jungers/content/home). UCLouvain.
- [Prof. Sophie Haesaert](https://www.sofiehaesaert.com). Eindhoven University of Technology.


##### Student supervision

###### Completed
- Luke Rickard. "Sample-based Control of Discrete-time Hybrid Systems with Non-Gaussian Noise". With [Prof. Alessandro Abate](https://www.cs.ox.ac.uk/people/alessandro.abate/home.html). PhD AIMS project. 
- John Ryan. "Reinforcement Learning for Space Operations". With [Prof. Alessandro Abate](https://www.cs.ox.ac.uk/people/alessandro.abate/home.html). MSc thesis.
- Thomas Koeck. "RL-based Attitude Control Problem". With [Prof. Alessandro Abate](https://www.cs.ox.ac.uk/people/alessandro.abate/home.html). MSc thesis.
- Ming Ow. "Data-driven optimisation algorithms: trading feasibility with performance". With [Prof. Kostas Margellos](https://kostasmargellos.github.io/). MSc thesis.


