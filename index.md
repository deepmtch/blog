---
layout: default
---
<html lang="en">
<head>
  ...
</head>
<body>
  ...
  <div class="content">
    <h1><p>Generated Blog Title</p></h1>
    ...
    <!-- Add this section to list your posts -->
    <div class="posts">
      {% for post in site.posts %}
      <article class="post">
        <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
        <p>{{ post.excerpt }}</p>
      </article>
      {% endfor %}
    </div>
    ...
  </div>
</body>
</html>
