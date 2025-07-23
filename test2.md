---
layout: page
title: /test
---

{{ site.data.soundboardio-superbobo.soundboardio.name }}
---

<div id="soundboard">
    {% for tile in site.data.soundboardio-superbobo.soundboardio.tiles %}
    <div class="sound-tile">
        <button onclick="playSound('{{ tile.filename }}')">{{ tile.name }}</button>
    </div>
    {% endfor %}
</div>

<audio id="audio-player" src="" hidden></audio>

<script>
    // Function to play the sound
    function playSound(filename) {
        const audioPlayer = document.getElementById('audio-player');
        audioPlayer.src = '/assets/sounds/' + filename;
        audioPlayer.play();
    }

    // Play sound if anchor link is present
    document.addEventListener('DOMContentLoaded', () => {
        const hash = window.location.hash.substring(1); // Get the anchor link without '#'
        if (hash) {
            playSound(hash);
        }
    });
</script>