---
layout: default
title: ise.pc-cdn.de - Quellennachweise 
---
{% include header.html %}
{% include navigation.html %}

<div id="home">
  <h1>used images</h1>
  <ul class="posts">
    {% for post in site.site %}
      <li>
       <span>
          {{ post.date | date_to_string }}
       </span> &raquo; 
       <a href="{{ site.url }}">
          <img src="/assets/img/bg/overlay-pattern.png" 
           style="background-image: url(/assets/img/post-thumbnails/{{post.thumbnail}})" 
           width="150" height="150" alt="{{ site.title }}"> 
       {{ site.title }}</a>
          </li>
    {% endfor %}
  </ul>
</div>
{% include footer.html %}