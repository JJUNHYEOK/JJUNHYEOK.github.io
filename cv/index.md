---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
# layout: default
# ---

---
layout: home
---

[Home](/) | [Blog](/blog/)

{{ site.name }}
{{ site.description }}

... CV 내용 계속 ...

---

## Recent Blog Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>

[블로그 전체 보기](/blog/)