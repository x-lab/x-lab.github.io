---
title: "News"
layout: textlay
excerpt: "XLab at Advanced Institute of Information Technology."
sitemap: false
permalink: /news.html
---

# News

{% for article in site.data.news %}
<p> <b> {{ article.date }} </b> <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
