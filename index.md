---
layout: index
title:
tagline:
---
{% include JB/setup %}

情報検索（Information Retrieval）と関連分野の国際研究動向を日本語ツイートで紹介します。[リソースガイド](./resources.html)も作成中です。また、国内外の研究者をゲストにお招きしたポッドキャストを配信します（おやすみ中）。[サイトについて](./about.html)

----
[重要な日程](./importantdates.html)

----

{% for post in site.posts %}
<p>{{ post.date | date_to_string }}<br/>
<a style="font-size:150%" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }} ({{ post.tagline }})</a><br/>
<span>{{ post.description }}</span></p>
{% endfor %}
