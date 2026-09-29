
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Tum Se - Music & Lyrics Player</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: Arial, sans-serif;
    color: white;
    background: linear-gradient(135deg, #130020, #4b125c, #080b25);
    padding: 20px;
}

.player {
    width: 100%;
    max-width: 430px;
    text-align: center;
    padding: 30px 24px;
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.15);
    border-radius: 25px;
    box-shadow: 0 15px 45px rgba(0,0,0,0.4);
}

.cover {
    width: 180px;
    height: 180px;
    margin: 0 auto 22px;
    border-radius: 50%;
    background: linear-gradient(135deg, #fc5c7d, #6a82fb);
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 70px;
    box-shadow: 0 0 30px #a34cfa66;
}

.cover.playing {
    animation: rotate 7s linear infinite;
}

@keyframes rotate {
    to { transform: rotate(360deg); }
}

h1 {
    font-size: 27px;
    margin-bottom: 8px;
}

.artist {
    color: #d5c1e8;
    margin-bottom: 24px;
}

.lyrics-box {
    min-height: 130px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 20px 0;
    padding: 18px;
    border-radius: 15px;
    background: rgba(0,0,0,0.22);
}

#lyrics {
    font-size: 21px;
    line-height: 1.6;
    color: #ffffff;
    transition: opacity 0.3s;
}

.controls {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin: 20px 0;
}

button {
    border: none;
    border-radius: 30px;
    padding: 13px 25px;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
}

#playBtn {
    background: #d75cff;
    color: white;
}

#playBtn:hover {
    background: #b83be8;
}

#progress {
    width: 100%;
    accent-color: #d75cff;
    cursor: pointer;
}

.time {
    display: flex;
    justify-content: space-between;
    margin-top: 8px;
    font-size: 12px;
    color: #d5c1e8;
}

.note {
    margin-top: 20px;
    font-size: 12px;
    color: #cbb9da;
}
</style>
</head>

<body>

<div class="player">

    <div class="cover" id="cover">🎵</div>

    <h1>Tum Se ❤️</h1>
    <p class="artist">Romantic Music Player</p>

    <div class="lyrics-box">
        <p id="lyrics">Press Play to begin the music 🎶</p>
    </div>

    <audio id="audio" preload="metadata">
        <source src="background_music.wav" type="audio/mpeg">
        Your browser does not support audio.
    </audio>

    <div class="controls">
        <button id="playBtn">▶ Play Music</button>
    </div>

    <input type="range" id="progress"
           min="0" max="100" value="0">

    <div class="time">
        <span id="currentTime">0:00</span>
        <span id="duration">0:00</span>
    </div>

    <p class="note">
        Add your own authorized lyrics in the JavaScript section.
    </p>

</div>

<script>
const audio = document.getElementById("audio");
const playBtn = document.getElementById("playBtn");
const lyricsElement = document.getElementById("lyrics");
const cover = document.getElementById("cover");
const progress = document.getElementById("progress");

// Replace these examples with lyrics you are authorized to use.
// Each time is measured in seconds from the start of the audio.
const lyrics = [
    { time: 0, text: "Tum se kiran dhoop ki" },
    { time: 5, text: "tum se siyaah raat hai" },
    { time: 10, text: "tum bin main bin baat ka" },
    { time: 15, text: "tum ho tabhi kuch baat hai ❤️" },
    { time: 20, text: "enjoy the music ❤️" }
];

function formatTime(seconds) {
    if (!Number.isFinite(seconds)) return "0:00";

    const mins = Math.floor(seconds / 60);
    const secs = Math.floor(seconds % 60);

    return mins + ":" + String(secs).padStart(2, "0");
}

playBtn.addEventListener("click", async () => {
    if (audio.paused) {
        try {
            await audio.play();
            playBtn.textContent = "⏸ Pause Music";
            cover.classList.add("playing");
        } catch (error) {
            lyricsElement.textContent =
                "Could not play audio. Check your MP3 file.";
        }
    } else {
        audio.pause();
        playBtn.textContent = "▶ Play Music";
        cover.classList.remove("playing");
    }
});

audio.addEventListener("timeupdate", () => {
    const current = audio.currentTime;

    progress.value = audio.duration
        ? (current / audio.duration) * 100
        : 0;

    document.getElementById("currentTime").textContent =
        formatTime(current);

    document.getElementById("duration").textContent =
        formatTime(audio.duration);

    let currentLyric = null;

    for (const line of lyrics) {
        if (current >= line.time) {
            currentLyric = line;
        } else {
            break;
        }
    }

    if (currentLyric) {
        lyricsElement.textContent = currentLyric.text;
    }
});

progress.addEventListener("input", () => {
    if (Number.isFinite(audio.duration) && audio.duration > 0) {
        audio.currentTime =
            (Number(progress.value) / 100) * audio.duration;
    }
});

audio.addEventListener("ended", () => {
    playBtn.textContent = "▶ Play Again";
    cover.classList.remove("playing");
    lyricsElement.textContent = "Music ended ❤️";
});

audio.addEventListener("error", () => {
    lyricsElement.textContent =
        "Audio not found. Add background_music.mp3 to this folder.";
});
</script>

</body>
</html>
