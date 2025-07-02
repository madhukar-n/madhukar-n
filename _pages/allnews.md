---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
---

## News

<div class="jumbotron">
  {% if site.data.news == empty %}
    <p>{{No news}}</p>
  {% else %}
    {% for article in site.data.news %}
      <p>
        <b>{{ article.date }}</b><br>
        {{ article.headline }}
      </p>
    {% endfor %}
  {% endif %}
</div>

