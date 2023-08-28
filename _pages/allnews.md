---
title: "News"
layout: textlay
excerpt: "Stat Group at USC Marshall."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
{{ article.date }}<br>{{ article.headline | markdownify}}
{% endfor %}
