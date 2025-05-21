---
layout: page
title: /test
---

{{ site.data.soundboardio-superbobo.soundboardio.name }}

---

{% for tile in site.data.soundboardio-superbobo.soundboardio.tiles %}
{% assign id = tile.filename | split: "." | first  %}

<audio id="{{ id }}" src="{{site.url}}/soundboard/{{ tile.filename}}" preload="auto"></audio>
- <button onclick="document.getElementById('{{id}}').play();">{{ tile.name }}</button>

{% endfor %}