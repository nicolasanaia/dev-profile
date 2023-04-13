---
layout: page
title: Projetos
permalink: projects
---

<div>
  {% for post in site.posts %}
    <div class="flex space-x-2 py-1">
      <img class="w-1/2" src="{{site.baseurl}}/assets/projects/{{ post.title }}.svg">
      <div>
        <h3><a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a></h3>
        <div class="text-sm text-gray-400">{{post.date | date: "%B %-d, %Y"}}</div>
      </div>
    </div>
  {% endfor %}
</div>


