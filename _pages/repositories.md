---
layout: page
permalink: /repositories/
title: repositories
description: I have several lonely GitHub projects, patiently waiting for their first star. ⭐ If you want to be their hero, check them out <a href='https://scholar.google.com/citations?hl=en&user=D7wgsokAAAAJ'><b>here</b></a>! 😆
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
