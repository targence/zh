---
layout: default
---
  <div class="header">
    <h1>Posts</h1>
  </div>
  <div class="content">
    {% for post in site.posts %}
      <div class="listing">
      	<hr class="slender">

      	<a href="{{ post.url | prepend: site.baseurl }}"><h4 class="contrast">{{ post.title }}</h4></a>
      	<span class="smaller">{{ post.date | date: "%H:%M:%S, %B %-d, %Y" }}</span>  <br/>
		<div>{{ post.content }}</div>

      </div>
    {% endfor %}
  </div>
