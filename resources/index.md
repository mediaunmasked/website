---
title:  "Resources"
image: 'http://placehold.it/500x500'
---
<div class="scene-element scene-element--fadeUp10">
  <ul class="posts">
    {% for post in site.categories["resources"] limit: 24 %}
      <li class="post">
        <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" class="scene-element scene-element--fadeBig" style="background: url({{ site.url }}{{ site.baseurl }}{{ post.image }}) center center no-repeat;">
          <div class="post-details">
            <span class="post-date">{{ post.date | date: '%B %d'  }}</span>
            <span class="post-category">{{ post.categories }}</span>
          </div>
          <span class="post-title">{{ post.title }}</span>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
<div class="container scene-element scene-element--fadeDown10">
  <div class="center-align"><a href="{{ site.url }}{{ site.baseurl }}/sitemap" class="btn blue darken-4">View All Posts</a></div>
</div>