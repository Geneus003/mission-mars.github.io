---
layout: blog
title: Космос
permalink: /space/
---

<ul class="posts-ul">
  {% for post in site.categories.space %}
    {% if post.url %}
        <li>
          <div class="jumbotron">
            <a href="{{ post.url }}"><h1>{{ post.title }}</h1></a>
            <div class="container">
              <div class="row">
                <div class="col-md-8">
                  <img src="{{ post.image }}" class="img-thumbnail">
                </div>
                <div class="col-md-4">
                  <p class="post-description">{{ post.description }}... <a href="{{ post.url }}"><i>Читать дальше</i></a></p>
                </div>
              </div>
            </div>
          </div>
        </li>
    {% endif %}
  {% endfor %}
</ul>
