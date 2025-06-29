---
layout: default
title: Home
---

# syuusyuu9701 archive

漢検1級１９８点！！　満点取るまで生涯学習！！

All posts are listed below, sorted by date.

<hr>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
      <p><em>Posted on {{ post.date | date: "%B %d, %Y" }} in {% for category in post.categories %}{{ category | capitalize }}{% unless forloop.last %}, {% endunless %}{% endfor %}</em></p>
    </li>
  {% endfor %}
</ul>
