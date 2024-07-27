---
title: Site List
permalink: /sites
layout: default
---
| Site Name | Description |
|-----------|-------------|
{% assign websites = site.websites | sort: 'date' %}
{% for website in websites %}
| [{{website.title}}]({{website.uri}}) | {{website.desc}} |
{% endfor %}
