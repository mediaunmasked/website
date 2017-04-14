---
title: Media Unmasked - Tech Reviews, Tutorials, and Resources
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
<div class="wrapper scene-element scene-element--fadeUp10">
  <ul class="posts">
    {% for post in site.posts limit: 99 %}
      <li class="post">
        <a href="{{ post.url }}" class="scene-element scene-element--fadeBig" style="background: url({{ post.image }}) center center no-repeat;">
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
  <div class="center-align"><a href="{{site.url}}/sitemap" class="btn blue darken-4">View All Posts</a></div>
</div>