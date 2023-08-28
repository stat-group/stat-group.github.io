---
title: "News"
layout: textlay
excerpt: "Stat Group at USC Marshall."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news limit:10000 %}
{{ article.date }}
{{ article.headline | markdownify}}

{% endfor %}
