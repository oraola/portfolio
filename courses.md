---
layout: page
title: Courses
permalink: /courses/
---

{% assign items = site.courses | sort: "semester" | reverse %}
{% for c in items %}
- [{{ c.title }}]({{ site.baseurl }}{{ c.url }}) — {{ c.semester }}
{% endfor %}
