---
layout: page
title: Projetos
permalink: projects
---

<div>
  {% for post in site.posts %}
    <div class="flex items-center">
      <img class="object-scale-down h-10 w-10 mr-3" src="{{site.baseurl}}/assets/projects/{{ post.title }}.png">
      <div class="content-center mx-3">
        <h3><a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>
        <div class="text-sm text-gray-400">{{post.date | date: "%B %-d, %Y"}}</div>
      </div> 
    </div>
  {% endfor %}
</div>


