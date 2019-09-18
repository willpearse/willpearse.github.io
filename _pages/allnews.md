---
title: "Pearse Lab - News"
layout: textlay
excerpt: "Pearse Lab -- News"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
