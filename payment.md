# index.md
---
{% raw %}
<style>
  body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1);
    background-size: 200% 200%;
    animation: gradientAnimation 10s ease infinite;
  }
  @keyframes gradientAnimation {
    0% { background-position: 0% 0%; }
    50% { background-position: 100% 100%; }
    100% { background-position: 0% 0%; }
  }
  .content {
    position: relative;
    z-index: 1;
    color: white;
    padding: 20px;
    text-align: center;
  }
</style>
<div class="content">
  # Welcome to My Blog & Docs
  This is a simple blog and documentation site built with Jekyll. Check out the [Blog](blog.md), [About](about.md), or [Payment](payment.md) pages.

  ## Latest Posts
  {% for post in site.posts %}
    - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%b %d, %Y" }}
  {% endfor %}
</div>
{% endraw %}

---
