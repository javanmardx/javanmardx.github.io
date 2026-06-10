---
layout: home
title: خانه
---

## گاه‌نوشت‌های یک زریر

از 1385 تا هنوز.

### آخرین پست‌ها

<ul>
{% for post in site.posts limit:10 %}
  <li>
    <a href="{{ post.url | relative_url }}">
      {% if post.title and post.title != "" and post.title != "post" and post.title != "Untitled Post" %}
        {{ post.title }}
      {% else %}
        پست بدون عنوان - {{ post.date | date: "%Y/%m/%d" }}
      {% endif %}
    </a>
    <small>({{ post.date | date: "%Y/%m/%d" }})</small>
  </li>
{% endfor %}
</ul>

[مشاهده همه پست‌ها]({{ '/all-posts.html' | relative_url }})
