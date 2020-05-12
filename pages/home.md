---
layout: default
title: Postikard | Hello
permalink: /
nav: light
---

<section class="home-hero">
  <div class="pw-container">
    <div class="home-hero-content">
      <p>Send digital postcards to anyone from anywhere!</p>
      <p></p>
      <p></p>
      <span class="white-text">Coming soon!</span>
      <!-- <a class="btn-lrg btn-lrg-dark" href="{{ "/contact/" | relative_url }}">Contact us</a>-->
    </div>
  </div>
</section>

<section class="home-projects">
  <div class="pw-container">
    <h3><a name="projects"></a>Postikards</h3>
    <div class="home-projects-list">
      {% for item in site.data.projects.list %}
      <div class="home-project">
        <a href="{{ item.url }}" alt="{{ item.title }}">
          <img class="home-project-thumbnail" src="{{ item.thumbnail }}" />
          <h4 class="home-project-title">{{ item.title }}</h4>
          <p class="home-project-description">{{ item.description }}</p>
        </a>
      </div>
      {% endfor %}
    </div>
  </div>
</section>
