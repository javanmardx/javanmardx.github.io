---
layout: home
title: "خانه"
---

 **گاه‌نوشت‌های یک زریر** 

از 1385 تا هنوز.

## آخرین پست‌ها

<ul>
  {% for post in site.posts limit:10 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%Y/%m/%d" }})</small>
    </li>
  {% endfor %}
</ul>

[مشاهده همه پست‌ها]({{ '/all-posts.html' | relative_url }})