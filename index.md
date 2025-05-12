---
layout: home
title: Welcome to Study Notes
---

# 📚 Welcome to Study Notes!

This is a collection of my personal study notes and documentation. Here you'll find various topics I'm learning about and want to share.

## Recent Notes

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

## Categories

{% for category in site.categories %}
### {{ category[0] | capitalize }}
{% for post in category[1] %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
{% endfor %}

---

## About This Site

This site is built with Jekyll and hosted on GitHub Pages. All content is written in Markdown and automatically converted to HTML. 