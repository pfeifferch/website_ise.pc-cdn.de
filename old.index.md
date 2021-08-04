---
layout: default
title: ise.pc-cdn.de - Quellennachweise 
---

<div id="home">
  <h1>used images</h1>
  <ul class="posts">
    {% for post in site.posts %}
      <li>
       <span>
          {{ post.date | date_to_string }}
       </span> 
       <blockquote>
        <a href="{{ post.url }}">
          <img src="/assets/img/bg/overlay-pattern.png" 
           style="background-image: url(/assets/img/post-thumbnails/{{post.thumbnail}})" 
           width="150" height="150" alt="{{ post.title }}"> 
           {{ post.title }}</a>
       </blockquote>
       </li>
    {% endfor %}
  </ul>
</div>