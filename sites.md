---
title: Site List
permalink: /sites
layout: main
---
{% assign websites = site.websites | sort: 'date' %}
{% for website in websites %}
- [{{website.title}}]({{website.uri}}) - {{website.desc}}
{% endfor %}
