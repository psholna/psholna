---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults


---
layout: default
---

<div class="home">
  <h1 class="page-heading">Мои публикации</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%d.%m.%Y" }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>

</div>
