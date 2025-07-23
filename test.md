---
layout: page
title: /test
---

{{ site.data.soundboardio-superbobo.soundboardio.name }}

---

{% for tile in site.data.soundboardio-superbobo.soundboardio.tiles %}
{% assign id = tile.filename | split: "." | first  %}

<audio id="{{ id }}" src="{{site.url}}/soundboard/{{ tile.filename}}" preload="auto"></audio>
- <button onclick="playSound('{{ id }}');">{{ tile.name }}</button> <button onClick="copyToClipboard('{{ id }}');"><i class="fa fa-share" aria-hidden="true"></i>
</button>

{% endfor %}

<script>
    function playSound(id) {
        const audioPlayer = document.getElementById(id)
        audioPlayer.play();
    }

    function copyToClipboard(id) {
        // {{ site.url }} does not work here 
        navigator.clipboard.writeText('https://bobhome.cz/test/#' + id);
    }

    // Play sound if anchor link is present
    document.addEventListener('DOMContentLoaded', () => {
        const hash = window.location.hash.substring(1); // Get the anchor link without '#'
        if (hash) {
            console.log("play", hash)
            playSound(hash);
        }
    });

</script>