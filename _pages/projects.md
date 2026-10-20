---
layout: page
title: Projects
permalink: /projects/
description: Research and educational technology projects in computing education.
nav: true
nav_order: 1
---

My projects explore how **computing education**, **computational thinking**, and **generative AI** can connect research and teaching practice.

## Research and educational initiatives

<div class="projects">
  {% assign sorted_projects = site.projects | sort: "importance" %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>

## Research interests

- Generative AI for computing education
- Generative AI applied to programming education
- Introductory programming and computational thinking
- Educational technologies and teacher professional development

See my [publications](/publications/) for peer-reviewed research.
