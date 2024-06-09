---
layout: home
---

<h1>⚡️ AI Productivity: Tips, Tricks, and Tutorials ⚡️</h1>

<!-- Add this section to list your posts -->
<div class="posts">
  {% for post in site.posts %}
  <article class="post">
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
    <p><a href="{{ site.baseurl }}{{ post.url }}">Read More</a></p>
  </article>
  {% endfor %}
</div>


<style>
  body {
    font-family: Arial, sans-serif;
  }
  h1 {
    text-align: center;
    color: #333;
    font-size: 3em;
    margin-top: 20px;
  }
  .posts {
    margin: 20px 0;
  }
  .post {
    border-bottom: 1px solid #ddd;
    padding: 10px 0;
  }
  .post h2 {
    color: #007bff;
  }
  .post-meta {
    color: #555;
  }
  .icons {
    margin: 40px 0;
    text-align: center;
  }
  .icons h2 {
    font-size: 2em;
    color: #333;
  }
  .icon-gallery {
    display: flex;
    justify-content: center;
    gap: 40px;
    margin-top: 20px;
  }
  .icon-item {
    text-align: center;
  }
  .icon-item img {
    width: 100px;
    height: 100px;
  }
  .icon-item p {
    font-size: 1.2em;
    color: #555;
    margin-top: 10px;
  }
</style>
