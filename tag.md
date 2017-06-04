---
layout: page_no_title
permalink: /blog/tag/

---

<div class="tags-expo">
  <div class="tags-expo-list">
    {% for tag in site.tags %}
    <a href="#{{ tag[0] | slugify }}" class="tag btn btn-default btn-xs btn-tag "><span class="glyphicon glyphicon-tag" aria-hidden="true"></span> {{ tag[0] }}</a>
    {% endfor %}
  </div>
  <hr/>
  <div class="tags-expo-section">
    {% for tag in site.tags %}
    <h2 id="{{ tag[0] | slugify }}">{{ tag[0] }}</h2>
    <ul class="tags-expo-posts">

        <ul class="post-list">
    {% for post in tag[1] %}
      <li>
        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ post.date | date: date_format }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h2>
        <p>{{post.excerpt}}</p>
      
      </li>
    {% endfor %}
  </ul>
  <a href="#"><span class="glyphicon glyphicon-menu-up" aria-hidden="true"></span> Back to Top</a>
    </ul>
    {% endfor %}
  </div>
</div>