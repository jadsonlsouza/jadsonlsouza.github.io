---
layout: page
permalink: /repositories/
title: Repositories
description: My publicly available GitHub repositories and software projects.
nav: true
nav_order: 6
---

You can explore my publicly available source code on [GitHub](https://github.com/jadsonlsouza). This page lists my public repositories; private research code is not shown.

{% if site.data.repositories.github_users %}
## GitHub profile

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>
{% endif %}

{% if site.data.repositories.github_repos %}
## Public repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
