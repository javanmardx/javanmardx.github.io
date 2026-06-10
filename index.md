---
layout: page
title: خانه
---

## گاه‌نوشت‌های یک زریر

از 1385 تا هنوز.

### آخرین پست‌ها

<ul>
{% for post in site.posts limit:10 %}
  <li>
    <strong>{{ post.date | date: "%Y/%m/%d" }}</strong> -
    <a href="{{ post.url }}">
      {% if post.title and post.title != "" and post.title != "post" and post.title != "Untitled Post" %}
        {{ post.title }}
      {% else %}
        پست بدون عنوان
      {% endif %}
    </a>
  </li>
{% endfor %}
</ul>

<p><a href="{{ '/all-posts.html' | relative_url }}">مشاهده همه پست‌ها</a></p>
