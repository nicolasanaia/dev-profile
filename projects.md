---
layout: page
title: Projetos
permalink: projects
---

<div>
  {% for post in site.posts %}
    <div class="flex items-center justify-start">
      <img class="object-contain h-10 w-10" src="{{site.baseurl}}/assets/projects/{{ post.title }}.png">
      <div class="ml-3">
        <h3><a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>
        <div class="text-sm text-gray-400">{{post.date | date: "%B %-d, %Y"}}</div>
      </div> 
    </div>
  {% endfor %}
</div>


