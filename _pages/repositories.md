---
layout: page
permalink: /repositories/
title: Repositories
description: Here are my two repositories. <strong>jan-kula</strong>, which is my <em>work</em> repo and <strong>ExpShare</strong> which is my <em>private</em> repo. Check both of them out!
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
