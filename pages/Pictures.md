---
layout: post
title: Pictures
permalink: /pictures/
img: /assets/img/drawing_03.svg
description: Pictures paint a thousand words.
---

{% assign image_files = site.static_files | where: "image", true %}
{% for myimage in image_files %}
<img src="{{ myimage.path }}" alt="img"/>
<br>
<br>
{% endfor %}
