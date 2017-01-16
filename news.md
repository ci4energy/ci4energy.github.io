---
layout: page
title: News
permalink: /news/
weight: 5
---

<!-- <div class="news"> -->


  <ul class="post-list">
    {% for post in site.posts %}
	  <hr class="seperator">
      <li> <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span> <h3> <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title}}</a> </h3> <span class="post-brief">{{ post.brief }} </li>
      <hr class="seperator">
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

<!-- </div> -->
