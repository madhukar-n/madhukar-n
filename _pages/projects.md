---
title: "Projects"
layout: page
sitemap: false
permalink: /projects/
---


<div class="projects">
  {% for project in site.data.projects %}
    <div class="project-card">
      <img src="{{ project.image }}" alt="{{ project.title }} thumbnail">
      <h3>{{ project.title }}</h3>
      <p><strong>Collaborators:</strong> {{ project.collaborators | join: ", " }}</p>
      <p>{{ project.description }}</p>
      <p><a href="{{ project.link }}" target="_blank">View Project</a></p>
      <p><strong>Tags:</strong> {{ project.tags | join: ", " }}</p>
    </div>
  {% endfor %}
</div>
