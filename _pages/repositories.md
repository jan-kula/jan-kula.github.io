---
layout: page
permalink: /repositories/
title: Repositories
description: Edit the `_data/repositories.yml` and change the `github_users` and `github_repos` lists to include your own GitHub profile and repositories.
nav: true
nav_order: 3
---
{% if site.data.repositories.github_users %}

## GitHub users

<div class="row">
  {% for user in site.data.repositories.github_users %}

    <div class="col-md-6 mb-4">
      <h4 class="mb-2">
        <a href="https://github.com/{{ user }}" target="_blank" rel="noopener noreferrer">
          <i class="fa-brands fa-github"></i>
          {{ user }}
        </a>
      </h4>

      <p>
        {{ site.data.repositories.github_user_descriptions[user] }}
      </p>
    </div>

  {% endfor %}
</div>

{% endif %}
