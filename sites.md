---
title: Site List
permalink: /sites
layout: default
---
{% assign websites = site.websites | sort: 'date' %}
| Site Name | Description |
|-----------|-------------|
{% for website in websites %}
| [{{website.title}}]({{website.uri}}) | {{website.desc}} |
{% endfor %}
